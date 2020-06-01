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
      <input type="text" class="form-control" id="inputName" placeholder="Name" name="name">
    </div>
    <div class="form-group col-md-6">
      <label for="inputEmail4">Email</label>
      <input type="email" class="form-control" id="inputEmail4" placeholder="Email" name="email">
    </div>
  </div>
  <div class="form-group">
    <label for="messagearea">How can I help?</label>
    <textarea class="form-control" id="messagearea" rows="3" name="message"></textarea>
  </div>
    <button type="submit" class="btn btn-primary">Say Hello! <i class="far fa-handshake"></i></button>
</form>