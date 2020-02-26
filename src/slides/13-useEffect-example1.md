# useEffect()

```jsx
function Chat({ userId }) {
  useEffect(() => {
    subscribeToChat(userId)
  }, [])

  ...
 }
```