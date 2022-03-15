# test-htmlforms-netlify

<b>What is HTML Forms?</b>

A webform, web form or HTML form on a web page allows a user to enter data that is sent to a server for processing. Forms can resemble paper or database forms because web users fill out the forms using checkboxes, radio buttons, or text fields.

<b>What is Netlify?</b>

Netlify is a San Francisco-based cloud computing company that offers hosting and serverless backend services for web applications and static websites.

<b>Ways to deploy on Netlify?</b>

<ul>
  <li>Using repositories from Github</li>
  <li>Using and designing a template from Scratch</li>
  <li>Manual Deploy</li>
</ul>

<b>What are Netlify forms?</b>

Netlify comes with built-in form handling that’s enabled by default. Our build bots do it by parsing your HTML files directly at deploy time, so there’s no need for you to make an API call or include extra JavaScript on your site.

<i>Things needed to parse </i> <br>
`data-netlify="true"` <br>
`method="POST"`

Here's a sample code 

```<form name="contact" method="POST" data-netlify="true">
  <p>
    <label>Your Name: <input type="text" name="name" /></label>   
  </p>
  <p>
    <label>Your Email: <input type="email" name="email" /></label>
  </p>
  <p>
    <label>Your Role: <select name="role[]" multiple>
      <option value="leader">Leader</option>
      <option value="follower">Follower</option>
    </select></label>
  </p>
  <p>
    <label>Message: <textarea name="message"></textarea></label>
  </p>
  <p>
    <button type="submit">Send</button>
  </p>
</form>
```

<a href="https://docs.netlify.com/forms/setup/">Netlify Form and API documentation here</a>
