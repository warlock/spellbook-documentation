# Events

## Add listener:

```javascript
sb.on('bye', name => {
        console.log(`Bye  ${name} !`)
})
```

## Multi-listener:

```javascript
sb.on(['hi', 'hello'], name => {
        console.log(`Hi ${name}!`)
})
```

## Emit event:

```javascript
sb.emit('hi', 'master')
```

## Multi-emit event:

```javascript
sb.emit(['hi', 'bye'], 'master')
```

## Remove listener:

```javascript
sb.remove('hi')
```

