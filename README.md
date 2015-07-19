# road

yet another js router, reinvented the wheel

## Goals

example:

```javascript
var streets = {
  '/': HomeRouter,
  'user/:username': UserRouter
}
var road = Road(streets)
Road.init('/')
```
