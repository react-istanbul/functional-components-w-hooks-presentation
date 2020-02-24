## Note 2: effect cleanup
```jsx
useEffect(() => {
  subscribeUser(userID)

  return () => unsubscribeUser(userID) // will run on unmount
}, [])
```