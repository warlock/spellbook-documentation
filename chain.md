# Chain Methods

This method is usable from 0.1.x version.

```javascript
sb.chain([{ a: 'asdasd' }, { a: 35 }])
.reverse()
.toString()
.toJSON()
.filterBy({ a : 35 })
.first()
.repeatify(5)
.size()
.repeatify(10)
.toString()
.json()
.get('2')
.duplicate()
.repeatify(2)
.map(x => x + 1)
.contains(11)
.return()
```

-&gt; true

## Can chain any method from Spellbook

```javascript
sb.chain([{ a: 'hi' }, { a: 35 }])
.first()
.get('a')
.toUpperCase()
.return()
```

-&gt; "HI"

## For return a value can use method "value\(\)", "return\(\)", "v\(\)" or "r\(\)"

```javascript
sb.chain(100)
.numerator(2)
.mult(1002)
.toString()
.size()
.divide(2)
.sum(6)
.toString()
.split('.')
.map(sb.toInt)
.max()
.value()
```

-&gt; 8

## Playing with chain

```javascript
sb.chain([{ a: 'asdasd' }, { a: 35 }])
.reverse()
.toString()
.toJSON()
.filterBy({ a: 35 })
.first()
.repeatify(5)
.size()
.repeatify(10)
.toString()
.json()
.get('2')
.duplicate()
.repeatify(2)
.map(x => x + 1)
.value()
```

-&gt; \[11,11\]

## Chaining comparision and functions

```javascript
sb.chain(sb.range(1,5))
.size()
.isNumber()
.ifElse(
 () => "hello",
 () => "bye"
 )
.function(x => `Res: ${x}`)
.value()
```

-&gt; "Res: hello"

## Make a normal event

```javascript
sb.on('evrec', console.log)
```

### Make an event from chain

```javascript
sb.chain('message')
.on('evrec2', (x, y) => {
 console.log(`${y} : ${x}`)
})
.value()
```

-&gt; "message"

## Emit from chain

```javascript
sb.chain([{ a: 'asdasd' }, { a: 35 }])
.reverse()
.toString()
.toJSON()
.filterBy({ a: 35 })
.first()
.repeatify(5)
.size()
.repeatify(10)
.toString()
.json()
.get('2')
.duplicate()
.repeatify(2)
.map(x => x + 1)
.emit('evrec')
.value()
```

-&gt; Rec: 11  
-&gt; \[11,11\]

