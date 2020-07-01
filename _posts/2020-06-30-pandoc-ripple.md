---
layout: post
title:  "Almost 0 dependency local site"
permalink: /almost-no-depedencies
image: "assets/images/static-site.png"
description: "Tools to create documentation that is available locally"
categories: [ Technical Writing ]
tags: [ pandoc, lujnrjs ]
toc: true
---

I had to solve for a curious use case. Creating documentation that can be used locally, is easy for other to contribute to and has little to no dependencies. There were a lot of other requirements that ruled out options such as mkDocs or even using something like Jekyll.

After asking around in [#writethedocs](https://www.writethedocs.org/slack/) Slack I was given two ideas:

* [Pandoc](https://pandoc.org/) can be used to stitch files together into a semblance of a static site.
* [Lunr](https://lunrjs.com/guides/getting_started.html) can be used as an offline search.

With this information in hand I started researching. I was in that predicament other technical writers find themselves in. Do I have time to write this myself or can I find something that is open-source?

The two resources that I found and changed for my needs, [Rippledoc.py](http://www.unexpected-vortices.com/sw/rippledoc/index.html) and [Lunr-Index-and-Search-for-Static-Sites](https://github.com/BLE-LTER/Lunr-Index-and-Search-for-Static-Sites). I am not going to explain setup for each one, you can visit the [repo](https://github.com/tjperry07/pandoc-local-site) I made or visit each tool for more on configuration options. 

## Rippledoc

[Rippledoc](https://gitlab.com/uvtc/rippledoc) handles most of the work converting Markdown to HTML. This solved my problem of how do I take the markdown from contributors and convert it into an HTML site.

* Uses Pandoc Markdown
* Automatically create a table of contents
* Has previous and next links
* It will follow the folder paths for nested items.

To edit the script for my needs, I made most of my changes to `pandoc_process_file`. 

## Lunr search for static sites

After using Rippledoc the site worked great. I was able to navigate between files using a browser; the site built pretty quickly and there was no training required. But as the site gets larger how do people find information? That is where [Lunr-Index-and-Search-for-Static-Sites](https://github.com/BLE-LTER/Lunr-Index-and-Search-for-Static-Sites) came in. Just pass in the docs folder location and it builds the index for all the HTML files. Then add a search page and :boom: you're done.

### A few things to look out for

File paths in `rippledoc.py` is not straightforward, you will need to generate them as part of the script. To make sure the search file is available on every page, I added a [search path](https://github.com/tjperry07/pandoc-local-site/blob/master/docs/rippledoc.py#L362): 

```python
html_bef = html_before.replace('{{path-to-search}}', '../' * depth + 'search.html')
```

Then called it later when it [builds the body](https://github.com/tjperry07/pandoc-local-site/blob/master/docs/rippledoc.py#L475):


{% highlight html%}
{% raw %}
  <div id="nav">
    <a href="{{path-to-search}}">Search</a>
  </div>
{% endraw %}
{% endhighlight %}


To control the description and keywords for search I added a [YAML block](https://raw.githubusercontent.com/tjperry07/pandoc-local-site/master/docs/alan_bean.md) to the end of the file. Pandoc will read a YAML block anywhere as long as it has the three dashes, `---`. There are better ways to do this, but for this quick example it works.

```yaml
---
header-includes:
    <meta name="keywords" content="moon,shepard" />
    <meta name="description" content="Rear Admiral Shepard was one of the Mercury astronauts named by NASA in April 1959, and he holds the distinction of being the first American to journey into space." />
---
```

What you get is a static site that can use used offline. Use Lunr as a local JavaScript file, write standard CSS only and you can take your docs anywhere.


## GitHub

* [GitHub Repo](https://github.com/tjperry07/pandoc-local-site)

## Improvements

These are some ideas for improving the workflow.

* After `ripplydoc.py` is finished move the Markdown and HTML to seperate folders.
* Add more CSS so the local site is responsive
* Change Ripplydoc.py to use YAML metadata.
* Run the `build_index.js` each time the site is built.
* Move the search on the main page.

## Resources

A list of resources that helped me along the way.

### Pandoc

* <https://stackoverflow.com/questions/25410701/how-do-i-include-meta-tags-in-pandoc-generated-html>
* <https://github.com/eakbas/TSPW>
* <https://www.romangeber.com/static_websites_with_pandoc/>

### Local Lunr search

* <https://github.com/BLE-LTER/Lunr-Index-and-Search-for-Static-Sites>
* <https://lunrjs.com/guides/index_prebuilding.html>
* <https://sentamal.in/articles/static-site-search-with-lunrjs/>
* <https://www.niamurrell.com/code/tutorials/2018-01-01-adding-search-engine-to-static-site/>

Todays cover art by: [https://blush.design/artists/vijay-verma](https://blush.design/artists/vijay-verma)