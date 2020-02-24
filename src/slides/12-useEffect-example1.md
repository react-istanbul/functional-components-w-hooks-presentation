# useEffect()

```jsx
function Welcome({ userID }) {
  useEffect(() => {
    fetchUserData(userID)
  }, [])

  return ...
 }
```