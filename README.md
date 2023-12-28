# Important Notes of this projects

## ReactNode
- `ReactNode` is a TypeScript type that represents a node in the **React component tree**.
- React components can render different types of content, such as text, elements, or fragments. 
- The `ReactNode` type is a way to express that a component can receive and render any type of content that is valid in the React virtual DOM.
  - `Node`: In the context of the virtual DOM, a node represents an element in the UI tree.

```tsx
interface MyButtonProps {
  /** The text to display inside the button */
  title: string;
  /** Whether the button can be interacted with */
  disabled: boolean;
}

function MyButton({ title, disabled }: MyButtonProps) {
  return (
    <button disabled={disabled}>{title}</button>
  );
}

export default function MyApp() {
  return (
    <div>
      <h1>Welcome to my app</h1>
      <MyButton title="I'm a disabled button" disabled={true}/>
    </div>
  );
}

```
