# multiple states


```jsx
function Dinosaur() {
  const [name, setName] = useState('')
  const [age, setAge] = useState(0)
  const [diet, setDiet] = useState('carnivore')

  return (
    <div>
    🦕 {name} {age} {diet}
    ...
  )
 }
```