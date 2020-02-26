# useEffect()

```jsx
function Chat({ userId }) {
  useEffect(() => {
    subscribeToChat(userId)

    return () => unsubscribeFromChat(userId)
  }, [userId])
  ...
 }
```