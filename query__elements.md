
# Querying Elements in JavaScript

## Examples

### Hide Elements
```javascript
hideElements(className) {
  const elements = document.querySelectorAll(className);

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
