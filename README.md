 # Res

 <img
 src='https://raw.githubusercontent.com/constraint-systems/res/master/public/res.gif'
 width="600"/>

Selectively pixelate an image using a compression algorithm.

https://res.constraint.systems


## compression as complexity

see `index.js` in `onLoad` =>

```
let t = document.createElement('canvas')
t.width = sp
t.height = sp
let tx = t.getContext('2d')

let x = i % cols
let y = Math.floor(i / cols)

tx.drawImage(c, x * sp, y * sp, sp, sp, 0, 0, sp, sp)

let complexity = t.toDataURL().length / (sp * sp)
```        