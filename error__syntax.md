# Syntax Error

## Identifier Multiple Declaration and Initialization as Constant

In this example the variable named `characters` has been declared and initialized multiple times.

```javascript
// Declaration and initialization of a constant variable named characters
const characters = 'lorem ipsum';

console.log('characters: ', characters);

// Declaration and initialization of a constant variable named characters for the second time
const characters = 'ipsum lorem';

console.log('characters: ', characters);
```



```javascript
/**
 *  Deno Error Message
 *
 *  The identifier/variable named characters has been declared
 *  and initialized multiple times when it must've been declared only once
 *  and because it is a constant, it must've been initialized only once
 */
error: Uncaught SyntaxError: Identifier 'characters' has already been declared
const characters = 'ipsum lorem';
      ^
```

