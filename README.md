# angular2-intro
Purpose of this page is to introduce great features of Angular2

## Web components

Angular2 logic is based on web components.
To make is simple : each element is independent and opens API callable by the other elements


## Router

It is the amazing part of angular is its router so easy to manage.

on the app.ts define router as it
```
{
  path: '/kitesurf/',
  component: kitesurf
}
```

kitesurf.ts component define router as it
```
{
  path: '/:location/',
  component: wind
}
```

wind.ts component define router as it
```
{
  path: ''
}
```
When you access ```/kitesurf/sanfrancisco``` automatically loading all 3 components setting ```location = sanfrancisco``` so that you know the wind in San Francisco
