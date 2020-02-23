# useState()


```jsx
function Counter() {
  const [count, setCount] = useState(0)
  
  function handleClick(e) {
    setCount(count + 1)
  }

  return (
      <>
        <p>You clicked {count} times</p>
        <button onClick={handleClick}>Click me</button>
      </>
   )
 }
```