# HTML Forms

Traditionally, the term 'form' has referred to a printed document that contains spaces for you to fill in information. HTML borrows the concept of a form to refer to different elements that allow you to collect information from visitors to your site.

### Why Forms?

The best known form on the web is probably the search box that sits right in the middle of Google's homepage.

In addition to enabling users to search, forms also allow users to perform other functions online. You will see forms when registering as a member of a website, when shopping online, and when signing up for
newsletters or mailing lists.

## Form Controls

There are several types of form controls that you can use to collect information from visitors
to your site.

![Res](images/fc.jpg)


### How Forms Work

A user fills in a form and then presses a button to submit the information to the server.

![Res](images/fw.jpg)

A form may have several form controls, eachgathering different information. The server
needs to know which piece of inputted data corresponds with which form element.

![Res](images/fd.jpg)


### Form Structure

`<form>`
Form controls live inside a `<form>` element. This element should always carry the action
attribute and will usually have a method and id attribute too.


`action`
Every `<form>` element requires an action attribute. Its value is the URL for the page on the
server that will receive the information in the form when it is submitted.

`method`
Forms can be sent using one of two methods: get or post. With the get method, the values from the form are added to the end of the URL specified in the action attribute. The get method is ideal for:
* short forms (such as search boxes)
* when you are just retrieving data from the web server (not sending information that 
should be added to or deleted from a database)


With the post method the values are sent in what are known as HTTP headers. As a rule of thumb you should use the post method if your form:
* allows users to upload a file
* is very long
* contains sensitive data (e.g. passwords)
* adds information to, ordeletes information from, a database If the method attribute is not
used, the form data will be sent using the get method.

`id`
We look at the id attribute on page 183, but the value is used to identify the form distinctly from other elements on the page (and is often used by scripts — such as those that check you have
entered information into fields that require values).


![Res](images/fs.jpg)

---

# Lists, Tables and Forms

### BULLET POINT STYLES list-style-type

The list-style-type property allows you to control the shape or style of a bullet point (also
known as a marker). It can be used on rules that apply to the <ol>, <ul>, and <li> elements.

**Unordered Lists**
For an unordered list you can use the following values:
* none
* disc
* circle
* square

**Ordered Lists**
For an ordered (numbered) list you can use the following values:

* decimal
* decimal-leading-zero
* lower-alpha
* upper-alpha
* lower-roman
* upper-roman