# Custom hooks

```jsx
function usePlayerLevel(playerId) {
  const [level, setLevel] = useState()

  useEffect(() => {
    getPlayerLevel(playerId).then(level => {
      setLevel(level)
    })
  }, [playerID])

  return level
}
```

```jsx
function playerCard({ playerId }) {
  const level = usePlayerLevel(playerId) 
  
  return <div>lvl: {level}</div>
}
```