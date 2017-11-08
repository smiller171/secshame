`searchItems([], STRING)` takes an array of items and a search key, and returns a filtered array of items.

This function should do fuzzy matching on all STRING fields in the array of items

## Errors
- [ ] If option is not a string, return `Error: invalid option: search term must be a string`
- [ ] If searching results in an error, pass that error up the stack
- [ ] If searching returns no results, return `Error: no results found` and an empty array
