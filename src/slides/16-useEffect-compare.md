```jsx
class Chat extends React.Component {
  componentDidMount() {
    subscribeToChat(this.props.userId)
  }
  
  componentDidUpdate(prevProps) {
    if (this.props.userId !== prevProps.userId) {
      unsubscribeFromChat(prevProps.userId)
      subscribeToChat(this.props.userId)
    }
  }

  componentWillUnmount() {
    unsubscribeFromChat(this.props.userId)
  }
}
```

```jsx
function Chat({ userId }) {
  useEffect(() => {
    subscribeToChat(userId)
    return () => unsubscribeFromChat(userId)
  }, [userId])
}
```