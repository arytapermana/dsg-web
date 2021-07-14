---
title: Contact
permalink: "/contact/"
layout: page
comments: false
---

<form action="https://formspree.io/f/xqkgqbpd" method="POST">    
<p class="mb-4">Please send your message to {{site.name}}. We will reply as soon as we can!</p>
<div class="form-group row">
<div class="col-md-6">
<input class="form-control" type="text" name="name" placeholder="Nama*" required>
</div>
<div class="col-md-6">
<input class="form-control" type="email" name="_replyto" placeholder="Alamat e-mail*" required>
</div>
</div>
<textarea rows="8" class="form-control mb-3" name="message" placeholder="Pesan*" required></textarea>    
<input class="btn btn-dark" type="submit" value="Kirim">
</form>
