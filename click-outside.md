# click-outside
-Whenever the user clicks outside the component, the component should close.

```js
import {useState,useRef,useEffect} from 'react'

export default function Profile(){
const [open,setOpen] = useState(false);
const ref = useRef(null);
useEffect(()=>{
    function handleClickOutside(e){
        if(!ref.current.contains(e.target)){
            setOpen(false)
        }
    }
    document.addEventListener('mousedown',handleClickOutside);
    return ()=>document.removeEventListener('mousedown',hanldeClickOutside)
},[]) //The return in useEffect is a cleanup function and it only runs when the component unmounts
return(
    <div ref={ref}>
        <button onClick={()=>setOpen(o=>!o)} >
            Profile
        </button>
        <div>
            {open && 
            <div>The content you wanna render</div>}
        </div>
    </div>
)
}
```