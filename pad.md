# pad

**sb.pad\(string, integer, string\)**  
Pads the string for a another string until arriving a total length:

```javascript
sb.pad('3',3,'0')
```

```text
-> "003"
```

```javascript
sb.pad('3',3,'foo')
```

```text
-> "fo3"
```

```javascript
sb.pad('3',33,'foo')
```

```text
->"foofoofoofoofoofoofoofoofoofoofo3"
```

