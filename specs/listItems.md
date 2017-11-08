`listItems({})` should return an array of objects.
## Options
```js
{
  filter: {},
  sort: {},
  search: STRING
}
```

### filter
Options for [`filterItems()`](specs/filterItems.md)

### sort
Options for [`sortItems()`](specs/sortItems.md)

### search
Options for [`searchItems()`](specs/searchItems.md)

## Errors
- [ ] All errors should be logged with `console.error()` and returned to the calling function as an error.
- [ ] Errors from dependent functions should be passed as-is up the stack
- [ ] JSON should be validated. Invalid JSON should return `ERROR: Invalid JSON`
- [ ] Does not validate format of options passed directly to child functions
- [ ] If latest items can't be retrieved from [`getItems()`](specs/getItems.md), an error should be returned as well as a hard-coded array of top items from [`getStaticItems()`](specs/getStaticItems.md) (will be stale)
- [ ] If an error is returned from [`getStaticItems()`](specs/getStaticItems.md), return an error with no array
- [ ] If an error is returned from [`filterItems()`](specs/filterItems.md), return the full array and an error
- [ ] If an error is returned by [`searchItems()`](specs/searchItems.md), return an error and the filtered array if a filter was applied, otherwise the full array
- [ ] If an error is returned by [`sortItems()`](specs/sortItems.md), return an error and an unsorted array (filtered and searched as applicable)

## Dependencies

* [`getItems()`](specs/getItems.md) returns a complete list of current items.
* [`getStaticItems()`](specs/getStaticItems.md) returns a hard-coded array of items if [`getItems()`](specs/getItems.md) fails.
* [`filterItems()`](specs/filterItems.md) returns a filtered array of items
* [`searchItems()`](specs/searchItems.md) returns a filtered array of items
* [`sortItems()`](specs/sortItems.md) returns a sorted array of items
