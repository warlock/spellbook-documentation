# isSet

**Check isSet values \(null, "", \[\], undefined\)**

```javascript
const a = ""
sb.isSet(a)
```

```text
-> false
```

sb.isEmpty && sb.get combination:

```javascript
const a = { 
  a: [
    { a: [1, 2, 3] }
  ],
  b: 4
}


sb.isSet(sb.get(a, 'a.0.a.1'))
```

```text
-> true
```

```javascript
sb.isEmpty(sb.get(a, 'a.0.b.1'))
```

```text
-> false
```

```javascript
sb.isSet(sb.get(a, 'a.0.b.1'))
```

```text
-> false
```

