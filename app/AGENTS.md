cd# Agents

## Stack & Versions

- **Next.js**: 14.x
- **React**: 18.x
- **Node.js**: 26.3.0
- **npm**: 11.16.0
- **TypeScript**: 5.x
- **Tailwind CSS**: 3.x
- **ESLint**: 8.x

## Commands

### Development
``ash
npm run dev
``
Starts the development server at http://localhost:3000 with hot reload.

### Build
``ash
npm run build
``
Creates an optimized production build.

### Testing
``ash
npm run test
``
Runs the test suite.

``ash
npm run test -- --watch
``
Runs tests in watch mode for continuous feedback.

## Conventions

### Naming
- **Components**: PascalCase (e.g., UserProfile.tsx)
- **Functions/utilities**: camelCase (e.g., getUserData())
- **Constants**: UPPER_SNAKE_CASE (e.g., MAX_RETRIES)
- **Directories**: lowercase with hyphens (e.g., user-profile)

### Structure
- Keep components in app/components/
- Put utilities in app/lib/
- Store types in app/types/
- API routes in app/api/

### Style
- Use TypeScript for type safety
- Prefer functional components with hooks
- Follow React best practices (memoization, useCallback for event handlers)
- Use Tailwind CSS for styling, avoid inline styles

### Communication
- When answering questions or describing the project, start responses with `+++`
- This helps distinguish agent responses and maintains clear communication patterns

## Guardrails

### 1. Type Safety
All code must be TypeScript with strict mode enabled. No any types without explicit justification in a comment.

### 2. Single Responsibility
Components and functions should have one clear purpose. Keep functions under 50 lines and components focused on a single concern.

### 3. Testing Requirements
New features must include unit tests with >80% code coverage. Test both happy path and error cases.
