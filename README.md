# Avan's home page

Plain static site. Served by GitHub Pages from the `main` branch root.

## Pages

- `index.html` - home
- `food/index.html` - food recommendations, index of lists
- `food/king-street/` - "Near King Street" list with a map

## Adding a restaurant

Add one object to `food/king-street/restaurants.json`:

```json
{
  "name": "Example Place",
  "address": "123 King St W, Toronto",
  "lat": 43.6470,
  "lng": -79.3890,
  "type": "takeout",
  "status": "rec",
  "order": "what to get",
  "note": "one line on why",
  "link": "https://..."
}
```

- `type`: `takeout` = takeout / lunch / dinner (filled pin), `sitdown` = lunch / dinner (hollow pin)
- `status`: `rec` = recommended (shown by default), `to-try` = on the research list, not tried yet (dashed pin, hidden unless "include places I haven't tried yet" is ticked)
- `order`, `note`, `link` are optional

## Adding a new list

Copy `food/king-street/` to a new folder, change the title and the map center in its `index.html`, empty its `restaurants.json`, and add a link on `food/index.html`.
