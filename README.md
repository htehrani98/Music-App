## export conditions:

- there is two ways to export a module:
- . default
- . assigned

examples:
> we have this function
```js
  function x() {}
```

if we wanna export it by default, we would say:
```js
  export default function x() {}
  // or
  export default x
```
if not, then say:
```js
  export function x() {}
```

## import conditions:

if a module has been exported by default, you should also import it by default
```js
  import x from '...'
```

if not, u should say:
```js
  import { x } from '..'
```

> all ways to import something:
```js
import defaultName from '...'
import { assignName } from '...'
import '...'
```
> all ways to export something:
```js
// if module is defined in another file :
export * from '...'
export { assignedName } from '...'
export defaultName from '...'

// if module is defined in current file
export default moduleName
export function FN(){}  /** OR **/ export const CONSTANT = "stuff"
```
