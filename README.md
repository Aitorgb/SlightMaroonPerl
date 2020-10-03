## Beers list

Create BeerList.js component, use it from App.js. This component sould:

fetch Beer list and render them into list elements:

* name
* description

Show "Loading..." while loading

api url: `https://ih-beers-api2.herokuapp.com/beers/`

## Random beer

Edit BeerList.js component, so this will start with an empty list, add a new random beer every 2 seconds until 10 beers.

Show "Loading..." while loading

api url: `https://ih-beers-api2.herokuapp.com/beers/random`

## Delete beer from list

Edit BeerList component, so a beer will be deleted when user click on it

It should not use the beers API

--------------------

### fetch

Use fetch instead of axios

```js
fetch('example.com/api/some.json')
  .then((response) {
      if (response.status !== 200) {
        console.log('Looks like there was a problem. Status Code: ' + response.status);
        return;
      }

      response.json().then(function(data) {
        console.log(data);
      });
    }
  )
  .catch(function(err) {
    console.log('Fetch Error :-S', err);
  });
```