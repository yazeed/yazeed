L# LTesting & Validation Rules
L
L## LTesting Philosophy
L- **Test-first mindset**: Consider testing requirements before implementation
L- **Quality over quantity**: Focus on meaningful tests rather than high coverage numbers
L- **Regression prevention**: Every test should prevent a specific regression
L- **Living documentation**: Tests serve as executable documentation
L
L## LTest Categories
L### LUnit Tests
L- **Function isolation**: Test functions in complete isolation
L- **Mock dependencies**: Mock all external dependencies
L- **Single responsibility**: Each test should verify one behavior
L- **Descriptive naming**: Use descriptive test names that explain the behavior
L
L### LIntegration Tests
L- **Component interaction**: Test how components work together
L- **API integration**: Test real API calls with test databases
L- **End-to-end flows**: Test complete user workflows
L- **Real dependencies**: Use real dependencies where practical
L
L### LEnd-to-End Tests
L- **User perspective**: Test from the user's point of view
L- **Critical paths**: Focus on critical user journeys
L- **Cross-browser**: Test across supported browsers
L- **Realistic data**: Use realistic test data and scenarios
L
L## LTest Structure
L### LTest Organization
L- **Colocation**: Keep tests next to the code they test
L- **Consistent naming**: Use consistent naming patterns (*.test.ts, *.spec.ts)
L- **Logical grouping**: Group related tests in describe blocks
L- **Setup/teardown**: Use beforeEach/afterEach for consistent setup
L
L### LTest Patterns
L- **Arrange-Act-Assert**: Follow AAA pattern in all tests
L- **Given-When-Then**: Use Gherkin syntax for complex scenarios
L- **Test doubles**: Use mocks, stubs, and spies appropriately
L- **Parameterized tests**: Use parameterized tests for data-driven scenarios
L
L## LReact Testing
L### LComponent Testing
L- **Render testing**: Test that components render correctly
L- **Interaction testing**: Test user interactions and state changes
L- **Props testing**: Test component behavior with different props
L- **Lifecycle testing**: Test component lifecycle methods
L
L### LHook Testing
L- **Hook isolation**: Test custom hooks in isolation
L- **State changes**: Test hook state changes and side effects
L- **Cleanup testing**: Test hook cleanup functions
L- **Error handling**: Test hook error scenarios
L
L## LTypeScript Testing
L### LType Testing
L- **Type assertions**: Test that functions return correct types
L- **Generic testing**: Test generic functions with different type parameters
L- **Interface compliance**: Ensure implementations match interfaces
L- **Type guards**: Test custom type guard functions
L
L### LRuntime Type Checking
L- **Schema validation**: Test runtime schema validation
L- **Input sanitization**: Test input validation and sanitization
L- **Error serialization**: Test error type serialization
L- **Type coercion**: Test automatic type coercion logic
L
L## LAPI Testing
L### LRequest/Response Testing
L- **Status codes**: Test correct HTTP status codes
L- **Response format**: Test response structure and content type
L- **Error responses**: Test error response formats
L- **Rate limiting**: Test rate limiting behavior
L
L### LData Validation
L- **Input validation**: Test input validation thoroughly
L- **Output validation**: Test output data structure
L- **Edge cases**: Test with malformed and edge case data
L- **Security testing**: Test for common security vulnerabilities
L
L## LPerformance Testing
L### LLoad Testing
L- **Concurrent users**: Test with multiple concurrent users
L- **Response times**: Monitor and assert on response times
L- **Resource usage**: Monitor memory and CPU usage
L- **Scalability testing**: Test system scalability limits
L
L### LPerformance Benchmarks
L- **Baseline metrics**: Establish performance baselines
L- **Regression detection**: Detect performance regressions
L- **Optimization validation**: Validate performance optimizations
L- **Real-world scenarios**: Test with realistic usage patterns
L
L## LAccessibility Testing
L### LScreen Reader Testing
L- **ARIA compliance**: Test ARIA attributes and roles
L- **Navigation testing**: Test keyboard navigation
L- **Content announcement**: Test screen reader announcements
L- **Focus management**: Test focus management in complex UIs
L
L### LVisual Testing
L- **Color contrast**: Test color contrast ratios
L- **Text scaling**: Test with different text sizes
L- **Touch targets**: Test touch target sizes
L- **Motion preferences**: Respect reduced motion preferences
L
L## LCross-Browser Testing
L### LBrowser Compatibility
L- **Supported browsers**: Test on all supported browsers
L- **Feature detection**: Test progressive enhancement
L- **Fallback behavior**: Test graceful degradation
L- **Polyfill testing**: Test polyfill functionality
L
L## LContinuous Integration
L### LAutomated Testing
L- **Pre-commit hooks**: Run tests before commits
L- **Pull request checks**: Run tests on pull requests
L- **Merge protection**: Prevent merging without passing tests
L- **Test reporting**: Generate and share test reports
L
L### LTest Environments
L- **Isolated environments**: Use isolated test environments
L- **Clean state**: Ensure clean state between tests
L- **Resource management**: Properly manage test resources
L- **Parallel execution**: Run tests in parallel for speed
L
L## LTest Maintenance
L### LTest Refactoring
L- **DRY principle**: Avoid duplication in test code
L- **Test utilities**: Create reusable test utilities
L- **Page objects**: Use page objects for UI tests
L- **Test data management**: Manage test data effectively
L
L### LTest Documentation
L- **Test documentation**: Document complex test scenarios
L- **Test naming**: Use clear, descriptive test names
L- **Test organization**: Organize tests logically
L- **Test discovery**: Make tests easy to find and understand
L
L## LDebugging Test Failures
L### LFailure Analysis
L- **Root cause analysis**: Find the root cause of test failures
L- **Flaky test identification**: Identify and fix flaky tests
L- **Test isolation**: Ensure tests don't interfere with each other
L- **Environment issues**: Identify environment-specific failures
L
L### LTest Reliability
L- **Deterministic tests**: Ensure tests are deterministic
L- **Race condition handling**: Handle async operations properly
L- **Timeout management**: Set appropriate timeouts
L- **Retry logic**: Implement retry logic for flaky operations
L
L## LTest Data Management
L### LTest Data Creation
L- **Realistic data**: Use realistic test data
L- **Edge cases**: Include edge case data in tests
L- **Data factories**: Use data factories for consistent data
L- **Data cleanup**: Clean up test data after tests
L
L### LData Privacy
L- **Sensitive data**: Avoid using real sensitive data in tests
L- **Data anonymization**: Anonymize test data
L- **Compliance**: Ensure test data complies with regulations
L- **Data isolation**: Isolate test data from production data






