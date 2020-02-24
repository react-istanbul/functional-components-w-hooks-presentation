# useEffect()

```jsx
function Chat({ userId }) {
  useEffect(() => {
    fetchUserData(userId)

    return () => unsubscribeFromChat(userId)
  }, [userId])
  ...
 }
```