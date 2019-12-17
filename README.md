# Test flow

Use to reproduce the error with `flow`.

## How to use

- `yarn install:all`
- `yarn lint-staged:all`
- `yarn flow` or `cd ./packages/test && yarn flow`

You will get this error:

```sh
Error ┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈ ../../node_modules/graphql/execution/execute.js.flow:3:39

Cannot resolve module iterall.

     1│ // @flow strict
     2│
     3│ import { forEach, isCollection } from 'iterall';
     4│
     5│ import inspect from '../jsutils/inspect';
     6│ import memoize3 from '../jsutils/memoize3';
```
