# Show me the code

```jsx
class ErrorBoundary extends React.Component {
  state = { hasError: false }

  static getDerivedStateFromError(error) {
    return { hasError: true }
  }

  componentDidCatch(error, errorInfo) {
    logError(error, errorInfo) // log the error here
  }

  render() {
    if (this.state.hasError) {
      return <p>💩</p> // show fallback UI instead of children
    }

    return this.props.children
  }
}
```