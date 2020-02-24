# useEffect()

```jsx
function Chat({ userId }) {
  useEffect(() => {
    fetchUserData(userId)
  }, [userId])

  ...
 }
```