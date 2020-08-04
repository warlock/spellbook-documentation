# isFunction

**Function type check:**

```javascript
sb.isFunction(() => {})
```

```text
-> true
```

```javascript
sb.isFunction(console.log)
```

```text
-> true
```

```javascript
sb.isFunction({})
```

```text
-> false
```

