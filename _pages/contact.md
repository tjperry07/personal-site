---
layout: page
title: Contact
permalink: /contact
comments: false
---



<form name="contact" action="/form-success.html" netlify-honeypot="bot-field" method="POST" netlify>
  <div class="form-row">
    <div class="form-group col-md-6">
      <label for="inputName">Name</label>
      <input type="text" class="form-control" id="inputName" placeholder="Name">
    </div>
    <div class="form-group col-md-6">
      <label for="inputEmail4">Email</label>
      <input type="email" class="form-control" id="inputEmail4" placeholder="Email">
    </div>
  </div>
  <div class="form-group">
    <label for="exampleFormControlTextarea1">How can I help?</label>
    <textarea class="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>
  </div>
    <button type="submit" class="btn btn-primary">Say Hello! <i class="far fa-handshake"></i></button>
</form>