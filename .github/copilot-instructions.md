# Instruções do GitHub Copilot

## Padrões de Código
- Use TypeScript para arquivos JS.
- Use arrow functions (`() => {}`) em vez de funções nomeadas.
- Utilize Tailwind CSS para estilização, mantendo classes consistentes.
- Nomes de variáveis devem ser em camelCase.

## Padrões de Estrutura
- Componentes React devem ser eficientes e reutilizáveis.
- Componentização é prioridade. Componentize sempre que puder.          
- Componentes não devem ter lógica e regras de negócio, apenas renderização.
- Toda lógica usada nos componentes deve ser criado em hooks customizados que pode estar na mesma pasta do componente.

## State Management
- Declare todos os states juntos
- Declare todos os hooks juntos
- Declare todos os useEffect juntos

## Props and Types

- Always define prop types (TypeScript interfaces or PropTypes)
- Use destructuring for props only when there's less then 3 props
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

## Testing

- Write tests for critical business logic
- Test user interactions, not implementation details
- Use React Testing Library for component tests
- Mock external dependencies appropriately

## Error Handling
- Implement Error Boundaries for graceful error handling
- Handle loading and error states in async operations
- Provide meaningful error messages to users
- Log errors appropriately for debugging
- Handle empty states with adequate icon, component and text
