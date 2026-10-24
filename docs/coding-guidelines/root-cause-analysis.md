L# root cause analysis & systematic problem solving
L
L## core philosophy
L- **always trace to root cause**: never apply band-aid fixes. every issue must be traced back to its fundamental origin.
L- **five whys method**: when encountering a bug, ask "why?" at least five times until reaching the true cause.
L- **hypothesis-driven debugging**: form hypotheses, then systematically test them through minimal reproducible examples.
L- **binary search debugging**: when dealing with complex systems, isolate problems by systematically dividing and conquering.
L
L## problem-solving framework
L### 1. immediate assessment
L- **reproduce reliably**: create minimal reproduction case before any investigation
L- **environment isolation**: test in clean environment to rule out external factors
L- **version pinning**: verify exact versions of all dependencies and tools
L
L### 2. systematic investigation
L- **single variable testing**: change only one thing at a time when debugging
L- **control groups**: compare working vs broken states side-by-side
L- **historical analysis**: use git bisect to find when issue was introduced
L- **dependency analysis**: check if issue correlates with specific package versions
L
L### 3. deep analysis
L- **call stack tracing**: follow execution path completely through all layers
L- **state inspection**: log/inspect all relevant state at each step
L- **network analysis**: monitor all network requests and responses
L- **performance profiling**: use tools to identify bottlenecks and memory issues
L
L### 4. root cause verification
L- **minimal fix validation**: verify fix works with minimal possible change
L- **regression testing**: ensure fix doesn't break existing functionality
L- **edge case coverage**: test all related scenarios, not just the reported issue
L
L## tool-specific debugging
L### react
L- **component hierarchy tracing**: use react devtools to inspect component tree
L- **state change tracking**: log all state updates and their triggers
L- **render cause analysis**: identify why components are re-rendering
L
L### typescript
L- **type narrowing**: use typeof/instanceof guards to narrow types systematically
L- **interface validation**: verify data structures match expected interfaces
L- **generic constraints**: ensure generic types are properly constrained
L
L### tailwind css
L- **utility class validation**: verify classes exist in current tailwind version
L- **css variable resolution**: check custom properties are defined and accessible
L- **build output inspection**: examine generated css for correctness
L
L### build tools
L- **cache clearing**: always clear all caches (vite, node_modules, etc.) first
L- **incremental testing**: build step-by-step, verifying each stage
L- **dependency resolution**: check package-lock/bun.lock for version conflicts
L
L## prevention & learning
L- **error logging**: implement comprehensive error boundaries and logging
L- **type safety**: use strict typescript settings to catch issues at compile time
L- **automated testing**: write tests that would have caught the issue
L- **documentation**: document root causes and solutions for future reference
L
L## when to stop
L- **verified fix**: issue is resolved and root cause is clearly identified
L- **comprehensive testing**: all related scenarios tested and working
L- **prevention measures**: safeguards implemented to prevent recurrence
L- **knowledge sharing**: findings documented and shared with team
L
L## red flags
L- **multiple simultaneous changes**: never make multiple changes without isolating each
L- **"quick fixes"**: any fix that doesn't address root cause is temporary at best
L- **"it works on my machine"**: issues must be reproducible and fixable in all environments
L- **ignoring warnings**: all warnings must be investigated and resolved
