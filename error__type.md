# Type Error



## Identifier Declared as Constant and Initialized Multiples Times



```javascript
// Declaration and initialization of a constant variable named characters
const characters = 'lorem ipsum';

console.log('characters: ', characters);

// Initialization of a constant variable named characters that has already been initialized
characters = 'ipsum lorem';

console.log('characters: ', characters);
```



```javascript
/**
 * Deno Error Message
 *
 * The identifier/variable named characters has been initialized
 * multiple times when it must've been initialized only 
 * once because it is a constant
 */

characters:  lorem ipsum
error: Uncaught TypeError: Assignment to constant variable.
characters = 'ipsum lorem';
           ^
```

