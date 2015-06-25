# road

another js router

## Goals

example:

```javascript
Road
.to('home')
.do({
  middleware: 'HomeWare',
  template: 'home', // it will get the innerHTML of $('#home-template')
  then: function(data, html) {
    // the data was transferred from the middleware as object
    // it will use `data` to render the template and store the renderred string in `html`
    Road.render($('#App'));
  }
})
```
