# road

another js router

## Goals

example:

```javascript
var opts = {
  'home': 'home',
  'fragment': '!'
}
var road = Road.init(opts);

road
.to('home')
.use('HomeWare', function() {
  var name1 = [1, 2, 3];
  var name2 = {a: 'a', b: 'b'};
  return {name1: name1, name2: name2};
})
.do({
  template: 'home', // it will get the innerHTML of $('#home-template')
  then: function(data, html) {
    // the data was transferred from the middleware as object
    // it will use `data` to render the template and store the renderred string in `html`
    Road.render($('#App'));
  }
})
```
