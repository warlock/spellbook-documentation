# getKeys

**sb.getKeys\(object, keys\)**

```javascript
const spells = {"fire": 5, "ice": 4, "electro": 6, "wind": 7}
sb.getKeys(spells, "fire");
```

```text
-> {"fire": 5}
```

```javascript
const spells = {"fire": 5, "ice": 4, "electro": 6, "wind": 7}
sb.getKeys(spells, ["fire", "wind"])
```

```text
-> {"fire": 5, "wind" : 7}
```

