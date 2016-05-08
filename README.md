# angular2-intro
Purpose of this page is to introduce great features of Angular2

## Web components

Angular2 logic is based on web components.
To make is simple : each element is independent and opens API callable by the other elements


## Router

The amazing part of angular is its simple but amazing router

app.ts component defines router as
```
{
  path: '/kitesurf/',
  component: kitesurf
}
```

kitesurf.ts component defines router as
```
{
  path: '/:location/',
  component: wind
}
```

wind.ts component defines router as
```
{
  path: ''
}
```
When you access ```/kitesurf/sanfrancisco``` angular2 automatically loads all 3 components, setting ```location = sanfrancisco``` so that you know the wind in San Francisco
