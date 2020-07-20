---
title: "Portfolio"
layout: default
permalink: "/portfolio"
toc: true
description: "Portfolio for Tatiana Perry"
---
## Rapid7

My job duties at Rapid7 are much different than they were at BigCommerce. While I still write documentation and help maintain API documentation, I find myself being able to help with training, processes and helping to make overarching decisions about documentation. Some of the work I am involved in includes:

* Creating metrics around the help documentation
* Writing product documentation. Some recent articles I have written (as of July 20, 2020):
  * <https://docs.rapid7.com/insightappsec/upgrade-an-on-premises-scan-engine>
  * <https://docs.rapid7.com/insightappsec/regenerate-engine-api-key>
  * <https://docs.rapid7.com/insightappsec/custom-options>
  * <https://docs.rapid7.com/insightappsec/how-to-configure-scan-scope>
  * <https://docs.rapid7.com/appspider/appspider-enterprise-jira-integration/#appspider-enterprise-jira-integration>
  * <https://docs.rapid7.com/insightappsec/appsec-chrome-extension>
* Advising on what an API and SDK MVP is
* What does a developer portal need to succeed
* Creating a plan to have open-source documentation for Metasploit.com
* Working with my teammates to close the content gap on tCell
* Researching and introduce new tools to make the documentation better
* Training my teammates on the more developer focused portions of our job
* Add tooling around our docs-as-code workflow
  * For those not famaliar with the command line use GitHub desktop
  * Create a branch with the ticket label and short description 
  * Work on your changes with frequent commits to save your work
  * Make a final commit with a short summary of changes
  * Push branch to documentation repo.
  * In the pull request description - go into detail on any changes made with a link back to the original ticket.
  * Add any labels needed
  * Assign the PR to the reviewers for that week
  * Setup codeowners to make sure all PRs were reviewed by someone on the docs team before publishing
  * No one can publish to master. Not even the codeowners
  * To filter out all the spam by being codeowners, integrated GitHub into a dedicated Slack channel and setup keywords so we could know when we were tagged as a reviewer or a review was re-requested
  * Create a Gmail filter to remove the "noise" since we have Slack notifications
  * Add in GitHub actions for Vale, First time committers and link checkers
  * Only create branches from master
  * Start every day by pulling from master
  * We don't care about the commit history
  * No need to squash. IF you want to squash use the button in the GitHub Repo, don't do it locally (its confusing locally)
* Leading weekly sessions on making the most of the new tools and figure out the process
* Converting the [style guide](https://github.com/tjperry07/ux-writing-linter-r7-old) to Vale
* Added [plugins](/current-writing-setup-june-2020) to help check for broken links and format the markdown
* Convert the [InsightIDR reference documentation](https://docs.rapid7.com/insightidr/log-search-api/) from Markdown to OpenAPI 3.0

<br>

<div class="row">
	<div class="col-sm-4">
		<div class="card">
			<div class="card-body">
				<h5 class="card-title">Metasploit Pro</h5>
				<p class="card-text">Metasploit Pro is the first project I tackled. <a data-toggle="collapse" href="#metasploitpro" role="button" aria-expanded="false" aria-controls="metasploitpro">
						Read More
					</a></p>
				<p>
				</p>
				<div class="collapse" id="metasploitpro">
					<p>
						The documentation needed an audit for gaps and a new site Information Architecture. I started by interviewing support, the engineering team that manages the product, and the previous writer. All of the information allowed me to create a plan to organize the site by a standard pen-testing workflow, along with user interface walkthroughs. I also organized the information by importance to the customer.
					</p>
				</div>
				<a href="https://metasploit.help.rapid7.com/docs" class="btn btn-primary" target="_blank">Metasploit Pro</a>
			</div>
		</div>
	</div>
	<!--Card one end-->
	<div class="col-sm-4">
		<div class="card">
			<div class="card-body">
				<h5 class="card-title">Metasploit Framework open-source</h5>
				<p class="card-text">Metasploit Framework is an open-source tool managed by Rapid7. The challenge with Metasploit Framework is that it needs documentation, and the documentation should be community-sourced. <a data-toggle="collapse" href="#metasploitframework" role="button" aria-expanded="false" aria-controls="metasploitframework">
						Read More
					</a></p>
				<p>
				</p>
				<div class="collapse" id="metasploitframework">
					<p>To help the community begin to self manage, I created a process around adding documentation to Metasploit Framework.</p>

					<p>There is a project on the repository where anytime a new feature is added, a card must be added. The card will include information about the feature and what should be documented.</p>

					<p>
						I also wrote <a href="https://github.com/tperry-r7/metasploit-framework/pull/4">new contributing guidelines</a>. They include a style guide, content examples, and tooling around the process. To help the community write documentation without me standing over them, I used a Vale <a href="https://github.com/errata-ai/vale" target="_blank">https://github.com/errata-ai/vale</a>, to convert the style into .yml files they can check the writing. I also recommend they install Markdown lint, <a href="https://github.com/DavidAnson/markdownlin" target="_blank">https://github.com/DavidAnson/markdownlint</a>, which verifies that the markdown is written in a consistent style.
</p>
				</div>
				<a href="https://github.com/rapid7/metasploit-framework" class="btn btn-primary" target="_blank">Metasploit Framework</a>
			</div>
		</div>
	</div>
	<!--Card two end-->
	<div class="col-sm-4">
		<div class="card">
			<div class="card-body">
				<h5 class="card-title">Training</h5>
				<p class="card-text">I am tasked with creating training around the more developer focused parts my job. <a data-toggle="collapse" href="#developertraining" role="button" aria-expanded="false" aria-controls="developertraining">
						Read More
					</a></p>
				<p>
				</p>
				<div class="collapse" id="developertraining">
					<p>The first significant piece of training was a crash course around documenting APIs.The team needed to get up to speed and quickly. I used Stoplight <a href="https://stoplight.io/" target="_blank">https://stoplight.io/</a>as the basis for the course because it provides a simple user interface you can use to compare to the Swagger.</p>
					<p> The class is built using Hugo and Netlify. <a href="https://github.com/tjperry07/ux-writing-training" target="_blank">https://github.com/tjperry07/ux-writing-training</a> </p>
				</div>
				<a href="https://ux-writing-r7.netlify.app/" class="btn btn-primary" target="_blank">UX Writer Training</a>
			</div>
		</div>
	</div> <!--Card three-->
</div>

<br>

## BigCommerce

At BigCommerce I was tasked with doing a full revamp of the BigCommerce developer site. This included rewriting all existing documentation, creating new spec files ,and finding a system that would work for both writers and the company. This meant working across the company with engineering, support ,and our developer advocate to create the best possible experience. As of May 31, 2020, that foundation is still in place.

Some of the work that I completed included:

* Rewrite of all developer documentation
* Creating new content to get the documentation up to date
* Rewriting API spec files
* Creating missing spec files
* Create site information architecture
* Figure out if the company should build a solution or go with a SaaS solution
* Writing and testing code for the documentation
* Verifying the accuracy of specification files

I have included several writing samples and specification files.

<div class="row">
	<div class="col-sm-4">
		<div class="card">
			<div class="card-body">
				<h5 class="card-title">Widgets writing sample</h5>
				<p class="card-text">A new feature was released that required an overview article, tutorial, code samples and a new API to be documented. <a data-toggle="collapse" href="#collapsewidgetwriting" role="button" aria-expanded="false" aria-controls="collapsewidgetwriting">
						Read More
					</a></p>
				<p>
				</p>
				<div class="collapse" id="collapsewidgetwriting">
					<p>
						BigCommerce released a new feature that would allow developers to make reuseable “blocks.”
						Customers could then add text or images to the “blocks,” making the stores easily customizable.
						The release required a lot of documentation to work in step with each other and strong collaboration with the project manager and engineering. The documentation included an API that needed to be checked for accuracy, a tutorial, code samples, and a full overview to explain the unfamiliar terms introduced.
					</p>
				</div>
				<a href="https://github.com/tjperry07/personal-site/tree/master/_portfolio_files/bigcommerce/widgets" class="btn btn-primary" target="_blank">Widget writing samples - GitHub</a>
			</div>
		</div>
	</div>
	<!--Card one end-->
	<div class="col-sm-4">
		<div class="card">
			<div class="card-body">
				<h5 class="card-title">Specification files</h5>
				<p class="card-text">One of my first tasks, when I started, was to update the specification files. <a data-toggle="collapse" href="#collapsespecfiles" role="button" aria-expanded="false" aria-controls="collapsespecfiles">
						Read More
					</a></p>
				<p>
				</p>
				<div class="collapse" id="collapsespecfiles">
					<p>
						My tasks included creating a style guide, adding samples, and making sure the information was accurate. I also found many APIs that were not documented and needed to be made public. I used a Stoplight to create the files and make the maintenance much easier for my self and others who wanted to edit the files. They were not built from code, so they needed to be handwritten. I created a style guide, worked with the engineering team, and created a system, so the specification files were kept up to date. The biggest project I completed was the Catalog.yml file. It required months of work and collaboration to make sure all the information was correctly documented. I created close to 15 spec files. I have linked to a few that set the tone for the API style guide.</p>
				</div>
				<a href="https://github.com/tjperry07/personal-site/tree/master/_portfolio_files/bigcommerce/spec_files" class="btn btn-primary" target="_blank">Spec files - GitHub</a>
			</div>
		</div>
	</div>
	<!--Card two end-->
	<div class="col-sm-4">
		<div class="card">
			<div class="card-body">
				<h5 class="card-title">Other writing samples</h5>
				<p class="card-text">These writing samples are a mixture of reference materials, tutorials, postman collections and concept articles. <a data-toggle="clapse" href="#collapseothersamples" role="button" aria-expanded="false" aria-controls="collapseothersamples">
						Read More
					</a></p>
				<p>
				</p>
				<div class="collapse" id="collapseothersamples">
					<p><strong>Developers Guide to Headless Commerce</strong> - This is a mixture of marketing and developer documentation. It is meant to inform and get the developers excited about headless commerce.
						The guide also includes several Postman collections meant to guide the user through a standard workflow. </p>
					<p><strong>Webhooks</strong> - Webhooks used to have a lot of confusion around them, and they were not well documented. I add some information on which events are available and created a quick tutorial based on an app our Developer Advocate had written. </p>
					<p><strong>Working with Storefront APIs</strong> - I noticed a gap in the content around how the Storefront APIs. Developers needed to know what they were and how to use them. This article is one of the earliest I wrote, and it's always a treat for me to compare this to the Widgets documentation that I wrote much later. I can see how far I have come. </p>
				</div>
				<a href="https://github.com/tjperry07/personal-site/tree/master/_portfolio_files/bigcommerce/other" class="btn btn-primary" target="_blank">GitHub</a>
			</div>
		</div>
	</div>
	<!--Card three-->
</div>