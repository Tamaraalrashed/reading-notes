# EJS

## Install

It's easy to install EJS with NPM.
```
$ npm install ejs
```
## Use
Pass EJS a template string and some data. BOOM, you've got some HTML.
```
let ejs = require('ejs');
let people = ['geddy', 'neil', 'alex'];
let html = ejs.render('<%= people.join(", "); %>', {people: people});
```
## CLI
Feed it a template file and a data file, and specify an output file.
```
ejs ./template_file.ejs -f data_file.json -o ./output.html
```
## Browser support
Download a browser build from the latest release, and use it in a script tag.
```
<script src="ejs.js"></script>
<script>
  let people = ['geddy', 'neil', 'alex'];
  let html = ejs.render('<%= people.join(", "); %>', {people: people});
</script>
```
## Docs
Example:
```
<% if (user) { %>
  <h2><%= user.name %></h2>
<% } %>
```
## Usage
```
let template = ejs.compile(str, options);
template(data);
// => Rendered HTML string

ejs.render(str, data, options);
// => Rendered HTML string

ejs.renderFile(filename, data, options, function(err, str){
    // str => Rendered HTML string
});
```

## Tags
- `<%` 'Scriptlet' tag, for control-flow, no output.
- `<%_`  ‘Whitespace Slurping’ Scriptlet tag, strips all whitespace before it.
- `<%=` Outputs the value into the template (HTML escaped)
- `<%-` Outputs the unescaped value into the template.
- `<%#` Comment tag, no execution, no output.


## Includes
ncludes are relative to the template with the `include` call. (This requires the 'filename' option.) For example if you have "./views/users.ejs" and "./views/user/show.ejs" you would use `<%- include('user/show'); %>`.

You'll likely want to use the raw output tag(`<%-`) with your include to avoid double-escaping the HTML output.

```
<ul>
  <% users.forEach(function(user){ %>
    <%- include('user/show', {user: user}); %>
  <% }); %>
</ul>
```
