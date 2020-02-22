# "Dumb" component

### AKA: Stateless, presentation or functional components


```jsx
const Dialog = ({ title, message, buttonText, handleConfirm  }) => {
  return (
    <div className='dialog'>
      <h1>{title}</h1>
      <p>{message}</p>
      <button onClick={handleConfirm}>{buttonText}</button>
    </div>
  )
}

```