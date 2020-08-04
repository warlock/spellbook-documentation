# filterBy

**Filter specific values from array of objects**

```javascript
var spells = [{ name : "fire", damage : 5 },{ name : "ice", damage : 4 }, { name : "water", damage : 5 }];
sb.filter(spells,{ damage : 5 });
```

```text
-> [{ name : "fire", damage : 5 },{ name : "water", damage : 5 }]
```

```javascript
var spells = [{ name : "fire", damage : 5 },{ name : "ice", damage : 4 }, { name : "water", damage : 5 }];
sb.filter(spells,{ name : "fire", name : "ice" });
```

```text
-> [{ name : "fire", damage : 5 },{ name : "ice", damage : 4 }]
```

