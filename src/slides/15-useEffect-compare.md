```jsx
class Welcome extends React.Component {
  componentDidMount() {
    fetchUserData(this.props.userID)
  }
  
  componentDidUpdate(prevProps) {
    if (this.props.userID !== prevProps.userID) {
      fetchUserData(this.props.userID);
    }
  }

  render() {
    ...
  }
}
```

```jsx
function Welcome({ userID }) {
  useEffect(() => {
    fetchUserData(userID)
  }, [userID])

  return ...
 }
```