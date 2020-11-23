# Reference Type

## Runtime Errors

### Example 1 - Identifier Multiple Declaration and Initialization as Constant

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



<br>

### Example 2 - Identifier Declared as Constant and Initialized Multiples Times



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

