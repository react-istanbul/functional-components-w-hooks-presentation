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
function playerCard({ playerID }) {
  const level = usePlayerLevel()
  
  return <div>lvl: {level}</div>
}
```