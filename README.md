# Avan's home page

Plain static site. Served by GitHub Pages from the `main` branch root.

## Pages

- `index.html` - home
- `food/index.html` - food recommendations, index of lists
- `food/king-street/` - "Near King Street" list with a map

## Adding a restaurant

Add one object to `food/king-street/restaurants.json` (list order = the # column):

```json
{
  "name": "Example Place",
  "address": "123 King St W, Toronto",
  "lat": 43.6470,
  "lng": -79.3890,
  "cuisine": "Thai",
  "distance": "450 m, 6 min walk",
  "distance_m": 450,
  "tried": ["Avan", "Marcus"]
}
```

- `distance` / `distance_m`: walking distance from 327 King St W (text shown, metres used for sorting)
- `tried`: any of `Avan`, `Anthony`, `Edison`, `Marcus`
- optional: `note`, `link`

## Adding a new list

Copy `food/king-street/` to a new folder, change the title and the map center in its `index.html`, empty its `restaurants.json`, and add a link on `food/index.html`.
