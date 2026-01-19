# DropDown
- you always render the component
- Just change the opacity and remove pointer events
```js
const [open,setOpen] = useState<boolean>('false');
<div className={`transition-all ease-in-out duration-200${open?'opacity-100 scale-100':'opacity-0 scale-95 pointer-events-none'}`}>

<div/>

```