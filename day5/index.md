# Concepts

## Add forms to a page
Forms let you collect and send data from one page to another, or from a page to a web server.
The following html will create a form for collecting first/last name and submit it to page1.html.
```html
<form action="page1.html">
    <label for="fname">First name:</label><br>
    <input type="text" id="fname" name="fname"><br>
    <label for="lname">Last name:</label><br>
    <input type="text" id="lname" name="lname">
    <input type="submit" value="Submit">
</form>
```

The default method for submitting data is a query string and it appears in the url like this
```text
www.mywebpage.com/page1.html?fname=Sean&lname=Rester
```

We can fetch these query string parameters with javascript like this
```javascript
const urlParams = new URLSearchParams(window.location.search);
const firstName = urlParams.get('fname');
const lastName = urlParams.get('lname');
```

# Project
Continue building your website, the rest of the class will be you making whatever you want.
During this time I will be demonstrating how to do various things that people ask and helping
with issues on websites.