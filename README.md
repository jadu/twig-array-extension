# Array Twig Extension

Filters to work with arrays prior to markup output, allowing you to exclude known keys, or only return specified keys. The filters are designed to be very permissive and won't throw any warnings or errors if the supplied keys do not exist.

Typically used in conjunction with Pulsar's attribute parser extension.

## Exclude from Array

Returns a filtered array with the specified keys removed.

Multiple items can be provided, space separated.

```twig
arrayToModify|exclude('itemToExclude')
```

## Only from Array

Returns only the items present in the filter list based on a case insensitive search

Multiple items can be provided, space separated.

```twig
arrayToModify|only('itemToInclude')
```
