# uniqBy

**Get unique values from array using specific object key**

Alternative name: unq.

```javascript
var spells = [{ name : "fire", damage : 5},{ name : "ice", damage : 5}];
sb.uniqBy(spells,"name");
```

```text
-> [ 'fire', 'ice' ]
```

```javascript
sb.uniqBy(spells,"damage");
```

```text
-> [ 5 ]
```

