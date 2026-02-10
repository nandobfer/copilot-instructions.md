# React Development Guidelines

## Code Style and Conventions

- Use functional components with hooks instead of class components
- Prefer TypeScript for type safety when available
- Use descriptive and meaningful variable names
- Follow camelCase for variables and functions, PascalCase for components

## Component Structure

- Keep components small and focused on a single responsibility
- Extract reusable logic into custom hooks
- Use composition over inheritance
- Place components in their own files with the same name as the component

## State Management

- Use `useState` for local component state
- Use `useEffect` for side effects
- Use `useContext` for sharing state across components
- Consider using `useReducer` for complex state logic
- Prefer state colocation - keep state as close to where it's used as possible

## Props and Types

- Always define prop types (TypeScript interfaces or PropTypes)
- Use destructuring for props
- Provide default values for optional props
- Keep prop drilling to a minimum

## Hooks Best Practices

- Only call hooks at the top level of components
- Follow the "Rules of Hooks"
- Name custom hooks with "use" prefix
- Memoize expensive computations with `useMemo`
- Memoize callbacks with `useCallback` when passing to optimized child components

## Performance

- Use React.memo() for expensive components that receive the same props frequently
- Avoid inline function definitions in JSX when passing to child components
- Use lazy loading for routes and heavy components
- Keep component render logic pure and fast

## File Organization

- Group related components in feature folders
- Keep utility functions in separate files
- Use index files for cleaner imports
- Separate business logic from UI components

## Testing

- Write tests for critical business logic
- Test user interactions, not implementation details
- Use React Testing Library for component tests
- Mock external dependencies appropriately

## Styling

- Use consistent styling approach (CSS Modules, styled-components, or Tailwind)
- Keep styles modular and component-scoped
- Avoid inline styles unless necessary for dynamic values
- Use CSS variables for theming

## Error Handling

- Implement Error Boundaries for graceful error handling
- Handle loading and error states in async operations
- Provide meaningful error messages to users
- Log errors appropriately for debugging
