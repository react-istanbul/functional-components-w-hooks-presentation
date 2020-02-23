##Note: Array destructuring
```jsx
  var countStateVar = useState(0) // Returns a pair
  var count = countStateVar[0] // First item in a pair
  var setCount = countStateVar[1] // Second item in a pair

  // or

  const [count, setCount] = useState(0)
```