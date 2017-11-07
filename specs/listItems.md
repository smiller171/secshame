`listItems({})` should return an array of objects.
### Options
```
{
  filter: {},
  sort: {},
  search: STRING
}
```

## filter
Options for [`filterItems()`](specs/filterItems.md)

## sort
Options for [`sortItems()`](specs/sortItems.md)

## search
Options for [`searchItems()`](specs/searchItems.md)

### Dependencies

should call [`getItems()`](specs/getItems.md) to get a complete list, and be passed through [`filterItems()`](specs/filterItems.md), [`searchItems()`](specs/searchItems.md), and [`sortItems()`](specs/sortItems.md) as needed to parse results.
