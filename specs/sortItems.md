`sortItems([], {})` takes an array of items and an `options` object and returns a sorted array of items.

## Options
```
{
  Key: STRING,
  Sort: STRING
}
```

### valid keys:
`company`, `bizType`, `issueType`, `reportDate`, `lastValidated`, `resolvedDate`, `sevRate`, `annoyRate`, `funnyRate`

### valid sorts:
`high`, `low`  
high indicates higher to lower or alphabetical  
low indicates lower to higher or reverse alphabetical

### default
```json
{
  "Key": "sevRate",
  "Sort": "high"
}
```

## Errors
- [ ] If options are invalid, return an error
- [ ] If sorting returns an error, pass that up the stack
