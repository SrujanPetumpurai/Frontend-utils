# Transition & Transform property
### Transition
- Provides a way to smoothly animate one or more properties
- animation behaviour

### Example
```js
.box{
    height:200px;
    width:200px;
    background:#ffff24;

    transition-property:width; //What property this transition is for
    transition-duration:2s;//How long the transition should last
    transition-timing-function:ease;//How the transition should behave
    transition-delay:0s;//After how long the transition should start
}
.box:hover{
    width:400px
    background-color:coral;
}
```
#### ShortHand
```js
transition:width 2s ease 0s,background-color 3s linear 1s; //Transition of multiple properties
transition:all 2s ease; //In case all the transition properties are the same
```

### Transform
- Visual change(scale,move,rotate,skew)

### Example
```js
.box{
    height:200px;
    width:200px;
    background:#ffff24;
}
.box:hover{
    transform: translate(20px, 10px);//Move
    transform: scale(1.1);//Grow
    transform: scale(0.9);//Shrink 
    transform:rotate(45deg);//Rotate
    transform: skew(10deg, 5deg);//Skew
    transform: translateY(-4px) scale(1.05);//Multiple

}
```
- *translate* moves the element in x or y axis.