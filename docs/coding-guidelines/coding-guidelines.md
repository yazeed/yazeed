# yazeed's coding guidelines

> General guidelines (older, tool-agnostic). Where they disagree with `~/.claude/CLAUDE.md` or a
> project's `CLAUDE.md` (e.g. zee works on `main` without PRs), those win.

## rules organization
this project uses a comprehensive ruleset organized by category. each category has its own detailed rules file:

- **[root cause analysis](root-cause-analysis.md)** - systematic problem-solving and debugging
- **[technology stack](tech-stack-rules.md)** - react, typescript, tailwind, bun, supabase, etc.
- **[code quality](code-quality-rules.md)** - formatting, naming, error handling, testing
- **[project management](project-management-rules.md)** - git workflow, planning, communication
- **[testing & validation](testing-validation-rules.md)** - unit, integration, e2e testing
- **[performance optimization](performance-optimization-rules.md)** - core web vitals, optimization
- **[security & reliability](security-reliability-rules.md)** - authentication, data protection
- **[documentation & communication](documentation-communication-rules.md)** - technical writing, knowledge sharing
- **[development environment](development-environment-rules.md)** - tools, ide, local setup
- **[deployment & production](deployment-production-rules.md)** - ci/cd, monitoring, operations

**reference these specific rule files for detailed guidance on each area.**

## project & code guidelines

### project
- always be conscious of the path(pwd) you're running commands on/from
- use bun as the exclusive package manager - no npm, yarn, or pnpm
- use bun run typecheck, bun lint, and bun test for checking code quality
- always start working on a clean branch, never push unnecessary files
- use github flow for releases
- use if not exists for new database migrations when applicable
- when multiple solutions exist, share all options for informed decision-making

### code quality
- prefer explicit code over implicit (even if more verbose)
- use functional approach with simple atomic functions without side-effects
- always read documentation before using unfamiliar functions
- keep files small and focused (< 100 lines per file)
- keep code colocated but avoid over-engineering folder structures
- use modern javascript/typescript features: import/export, arrow functions, const/let
- write readable, understandable code - not clever code
- write comments explaining what code does (especially non-obvious logic)
- all code must be typed - avoid `any` types (never use them)
- use ternary operators sparingly - prefer early returns over if/else
- prefer async/await over raw promises
- group all imports at the top of files, let ide auto-sort them
- write tests for new functions (even llm-generated tests are acceptable for basic functionality)

### dependencies
- minimize circular dependencies
- never disable eslint or typescript rules without absolute necessity

## react guidelines

### component architecture
- use pascalcase for component files and named exports
- use camelcase for hook files and named exports
- define simple, non-reusable types inline
- define complex/reusable types in dedicated `types.d.ts` files
- never expose sensitive environment variables to client-side code

### state management
- use supabase for user settings and state - avoid localstorage
- always use usememo and usecallback to prevent unnecessary re-renders
- always provide loading and error states
- always provide zero-state for all lists
- never use javascript for mobile/desktop detection - use tailwind responsive prefixes

### lifecycle & effects
- use useeffect sparingly - prefer avoiding it when possible
- always double-check usememo/usecallback/useeffect dependencies
- add comments for omitted dependencies explaining why they're omitted

### best practices
- prefer semantic html for buttons, labels, etc. - avoid div overuse
- one component per file
- never create components inside render functions
- never create static data inside render functions
- never use simple array indices as react keys
- only use `condition &&` checks in render when `condition` is boolean
- prefer server components first, client components only when needed
- mobile-first design - start with smallest screens
- use only tailwind css for styling
- utilize tailwind responsive prefixes instead of custom breakpoint logic
- no hardcoded pixel styles (use em instead of px)
- use supabase helper hooks for database queries, never use supabase client directly
- always explicitly check auth and throw errors for unauthenticated users in next.js server functions

## database guidelines

### schema design
- add custom typescript types for tables with jsonb columns
- include validation schemas for jsonb columns when shape is finalized

### migrations
- squash migrations into single files doing one thing only
- no sequential migrations that depend on each other

### queries
- write explicit queries - never use `select *`
- fetch only required columns
- implement and rigorously test row level security policies

### performance
- ensure appropriate database indexes for frequently queried columns

## development workflow

### git
- write clear, concise commit messages explaining changes
- write atomic commits representing single logical changes
- use github flow (rebase merges)
- small prs for specific features (< 500 lines of code)

### llms & ai
- prefer one prompt per file for better model understanding
- be explicit and detailed in prompts - don't be afraid of long prompts
- test prompts at least 10 times with same input (aim for 8-9/10 consistency)

## tool-specific rules

### ai coding assistants
- use llm sparingly - it's not a silver bullet
- prefer "ask" mode over agent mode with specific tasks
- proof-read and test ai output before committing
