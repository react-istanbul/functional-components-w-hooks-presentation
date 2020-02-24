# Custom hooks

```jsx
function playerCard({ playerID }) {
  const [level, setLevel] = useState()

  useEffect(() => {
    getPlayerLevel(playerId).then(level => {
      setLevel(level)
    })
  }, [playerID])

  return <div>lvl: {level}</div>
 }
```