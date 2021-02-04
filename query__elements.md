
# Querying Elements in JavaScript

## Examples

### Hide Elements

```javascript
hideElements(className) {
  const elements = document.querySelectorAll(`.${className}`);
  Object.values(elements).forEach(element => element.style.display = 'none');
},
```

<details>
  <summary>Explained</summary>
  <code>
```javascript
/**
 *  - Here's an example of a method that will take a CSS class name
 *    and it will hide the element(s) by setting their display to none. 
 */
hideElements(className) {
  const elements = document.querySelectorAll(`.${className}`);

  console.log('typeof elements: ', typeof elements);
  // typeof elementes: object

  console.log('elements: ', elements);
  /**
   * elements: NodeList [tr.additional-donation]
   *            0: tr.additional-donation
   *            length: 1
   */

  Object.values(elements).forEach(element => element.style.display = 'none');
},
```
</code>
</details>


