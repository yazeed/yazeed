L# technology stack rules & best practices
L
L## react 19 rules
L### component architecture
L- **server components first**: always start with server components, only use client components when necessary
L- **no default exports**: use named exports for all components (pascalcase naming)
L- **component composition**: prefer composition over inheritance
L- **props destructuring**: always destructure props in function parameters
L
L### state management
L- **supabase for persistence**: never use localstorage for important data
L- **minimal client state**: only use react state for ui-specific concerns
L- **state colocation**: keep state as close to where it's used as possible
L- **immutable updates**: always use immutable state updates
L
L### performance
L- **usememo for expensive computations**: wrap complex calculations
L- **usecallback for event handlers**: prevent unnecessary re-renders
L- **react.memo sparingly**: only memoize when re-renders are provably expensive
L- **key prop strategy**: never use array indices as keys
L
L### hooks
L- **custom hooks for logic**: extract reusable logic into custom hooks
L- **useeffect dependencies**: include all dependencies or use eslint disable with explanation
L- **cleanup functions**: always provide cleanup in useeffect when needed
L- **hook dependency arrays**: keep them minimal and accurate
L
L## typescript rules
L### LType Safety
L- **Strict mode**: Always use strict TypeScript settings
L- **No any types**: Never use `any` - find proper types or create interfaces
L- **Interface over type**: Use interfaces for object shapes, types for unions
L- **Generic constraints**: Properly constrain generic types
L
L### LType Definitions
L- **Colocate types**: Define types near their usage
L- **Shared types in types.d.ts**: Move reusable types to dedicated files
L- **Discriminated unions**: Use for complex state management
L- **Branded types**: Use for domain-specific primitive types
L
L### LError Handling
L- **Typed errors**: Create specific error types for different failure modes
L- **Result types**: Consider using Result<T, E> pattern for operations that can fail
L- **Error boundaries**: Implement React error boundaries for graceful failure
L
L## LTailwind CSS 4 Rules
L### LUtility Usage
L- **Semantic class names**: Use Tailwind's semantic color names (slate, gray, etc.)
L- **Responsive prefixes**: Always start mobile-first (sm:, md:, lg:)
L- **Consistent spacing**: Use Tailwind's spacing scale consistently
L- **Custom properties**: Define design tokens as CSS custom properties
L
L### LComponent Styling
L- **No arbitrary values**: Avoid `w-[123px]` - use design system values
L- **Layer organization**: Use `@layer` directives for proper CSS cascade
L- **Dark mode**: Implement proper dark mode with CSS custom properties
L- **CSS variables**: Define theme variables in :root and .dark
L
L### LPerformance
L- **Purge unused styles**: Ensure proper content paths for tree shaking
L- **CSS optimization**: Use Tailwind's built-in optimizations
L- **Bundle analysis**: Regularly check bundle size impact
L
L## LBun Rules
L### LPackage Management
L- **Bun.lock only**: Never commit package-lock.json or yarn.lock
L- **Latest versions**: Always use latest stable versions when installing
L- **Exact versions**: Use exact versions (^version) for reproducibility
L- **Workspace management**: Use bun workspaces for monorepos
L
L### LDevelopment Workflow
L- **bun run commands**: Use bun for all npm script execution
L- **Fast refresh**: Leverage bun's fast refresh capabilities
L- **Type checking**: Use bun's built-in TypeScript checking
L- **Hot reload**: Take advantage of bun's fast hot reload
L
L## LVite Rules
L### LBuild Configuration
L- **Minimal config**: Keep vite.config.ts minimal and focused
L- **Plugin ordering**: Order plugins logically (CSS first, then JS transforms)
L- **Asset optimization**: Configure proper asset handling for images/fonts
L- **Environment variables**: Use VITE_ prefix for client-side env vars
L
L### LDevelopment Server
L- **HMR configuration**: Disable overlay for better error handling
L- **Port management**: Use strictPort: false to avoid conflicts
L- **CORS handling**: Configure CORS properly for API calls
L- **Proxy setup**: Set up proper API proxies for development
L
L## LTanStack Router Rules
L### LRoute Configuration
L- **File-based routing**: Use TanStack Router's file-based routing
L- **Route parameters**: Strongly type route parameters
L- **Nested routes**: Properly structure nested route hierarchies
L- **Route guards**: Implement authentication guards at route level
L
L### LData Loading
L- **Loader functions**: Use loader functions for data fetching
L- **Error handling**: Implement proper error boundaries for routes
L- **Loading states**: Provide loading UI for async operations
L- **Cache management**: Leverage TanStack Query integration
L
L## LSupabase Rules
L### LDatabase Operations
L- **Row Level Security**: Always implement RLS policies
L- **Type safety**: Generate and use TypeScript types from database
L- **Connection pooling**: Use connection pooling for performance
L- **Migration strategy**: Use explicit migrations, never direct schema changes
L
L### LAuthentication
L- **Server-side verification**: Always verify auth on server-side
L- **JWT handling**: Properly handle JWT tokens and refresh
L- **Session management**: Implement proper session handling
L- **Security headers**: Set appropriate security headers
L
L### LReal-time Features
L- **Subscription management**: Properly clean up real-time subscriptions
L- **Connection handling**: Handle connection drops and reconnections
L- **Performance monitoring**: Monitor real-time feature performance
