# and

**With two values**

```javascript
sb.and(true, false)
```

```text
-> false
```

**Working with chain**

```javascript
const a = ['a']
const b = ['b']
sb.chain(a).contains('a').and(b).contains('c').value()
sb.chain(a).contains('a').and(b).contains('b').value()
```

```text
-> false
-> true
```

