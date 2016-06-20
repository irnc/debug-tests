# debug-tests
Bare bones setup to debug tests

## How to debug tests in WebStorm?

Add `$NODE_DEBUG_OPTION` to script you want to debug, so `package.json`
has a following section:
  
```json
{
  "scripts": {
    "test": "mocha $NODE_DEBUG_OPTION"
  }
}
```

1. Open _Run_ > _Edit Configurations..._ dialog.
2. Add New Configuration (Alt+Insert), a green plus button at top-left.
3. Select _npm_.
4. _Name_ is whatever, e.g. _test_.
5. For _Scripts_ select `test`.
6. Click _OK_.
7. _Debug_ this configuration using a _bug icon_ at top-right corner of
   the main window. 
