# Not

**Invert boolean value**

```javascript
sb.Not(true);
```

```text
-> false
```

**Use with chain**

```javascript
var spells = [{ name : "fire", damage : 5 },{ name : "ice", damage : 4 }, { name : "water", damage : 5 }];

sb.chain(spells).get("1").keys().contains("name").Not().value()
```

```text
-> false
```

