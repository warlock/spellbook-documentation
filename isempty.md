# isEmpty

**Check isEmpty values \(null, "", \[\], undefined\)** Alternative names: empty

```javascript
const a = ""
sb.isEmpty(a)
```

```text
-> true
```

sb.isEmpty && sb.get combination:

```javascript
const a = { 
  a: [
    { a: [1, 2, 3] }
  ],
  b: 4
}

sb.isEmpty(sb.get(a, 'a.0.a.1'))
```

```text
-> false
```

```javascript
sb.isEmpty(sb.get(a, 'a.0.b.1'))
```

```text
-> true
```

```javascript
sb.isEmpty(sb.get(a, 'a.0.b.1'))
```

```text
-> true
```

