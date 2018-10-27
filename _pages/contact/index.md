---
layout: page
title: Contact
permalink: /contact/
toggle: off
rank: 7
---


<form class="wj-contact" action="https://formspree.io/{{site.email}}" method="POST">
    <input type="email" name="email" placeholder="Enter your email">
  First name:<br>
  <input type="text" name="firstname"><br>
  Last name:<br>
  <input type="text" name="lastname">
  <input type="radio" name="application goal" value="MSc"> MSc<br>
  <input type="radio" name="application goal" value="PhD"> PhD<br>
  <input type="radio" name="application goal" value="Postdoctoral"> Postdoctoral fellow<br>
  <input type="radio" name="application goal" value="Work"> Employment <br>
  <input type="radio" name="application goal" value="Volunteer"> Volunteer
  <br>
  <textarea rows="10" cols="150" name="message" placeholder="Type your message here"></textarea>
  Attach a file (CV, coverletter). Merge multiple files into a single PDF. <input type="file" name="myFile">
  <button type="submit">Send</button>
</form>

<style>
form.wj-contact input[type="text"], form.wj-contact textarea[type="text"] {
    width: 100%;
    vertical-align: middle;
    margin-top: 0.25em;
    margin-bottom: 0.5em;
    padding: 0.75em;
    font-family: monospace, sans-serif;
    font-weight: lighter;
    border-style: solid;
    border-color: #444;
    outline-color: #2e83e6;
    border-width: 1px;
    border-radius: 3px;
    transition: box-shadow .2s ease;
}
form.wj-contact input[type="submit"] {
    outline: none;
    color: white;
    background-color: #2e83e6;
    border-radius: 3px;
    padding: 0.5em;
    margin: 0.25em 0 0 0;
    border: 1px solid transparent;
    height: auto;
}
</style>

