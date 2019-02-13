---
title: "Let's have a coffee"
permalink: "/lets-have-a-coffee.html"
---

<form action="https://formspree.io/{{site.email}}" method="POST">    
<p>Please send your message to {{site.name}}. </p>
<p>I like to hear new ideas, stories and help people and project!</p>
<p>I will come back to you soon!</p>
<div class="form-group row">
<div class="col-md-6">
<input class="form-control" type="text" name="name" placeholder="Name*" required>
</div>
<div class="col-md-6">
<input class="form-control" type="email" name="_replyto" placeholder="E-mail Address*" required>
</div>
</div>
<textarea rows="8" class="form-control mb-3" name="message" placeholder="Message*" required></textarea>    
<input class="btn btn-success" type="submit" value="Send">
</form>

<h2> Latest Blog Posts </h2>

{% for e in site.medium_posts %}

<div class="row">
  <h3>{{e.title}}</h3>
  {% endfor %}

</div>