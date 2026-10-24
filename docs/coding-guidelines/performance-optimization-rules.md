L# LPerformance & Optimization Rules
L
L## LPerformance Philosophy
L- **Proactive optimization**: Optimize early, but only after measuring
L- **User-centric metrics**: Focus on metrics that matter to users
L- **Sustainable performance**: Maintain performance as features grow
L- **Performance budgeting**: Set and enforce performance budgets
L
L## LCore Web Vitals
L### LLargest Contentful Paint (LCP)
L- **Optimize images**: Compress and serve images in modern formats
L- **Critical CSS**: Inline critical CSS to reduce render blocking
L- **Server response**: Optimize server response times
L- **Resource loading**: Prioritize loading of above-the-fold content
L
L### LFirst Input Delay (FID)
L- **JavaScript minimization**: Minimize and defer non-critical JavaScript
L- **Main thread blocking**: Avoid long-running JavaScript on main thread
L- **Input responsiveness**: Ensure UI remains responsive to user input
L- **Event handling**: Optimize event handlers and listeners
L
L### LCumulative Layout Shift (CLS)
L- **Stable layouts**: Reserve space for dynamic content
L- **Font loading**: Prevent font swap layout shifts
L- **Image dimensions**: Always specify image dimensions
L- **Dynamic content**: Handle dynamic content loading carefully
L
L## LReact Performance
L### LComponent Optimization
L- **Memoization strategy**: Use React.memo for expensive components
L- **Callback memoization**: Use useCallback for event handlers
L- **Dependency optimization**: Keep hook dependencies minimal
L- **Re-render analysis**: Use React DevTools Profiler to analyze renders
L
L### LState Management
L- **State colocation**: Keep state close to where it's used
L- **Derived state**: Avoid redundant state, compute from existing state
L- **State updates**: Batch state updates when possible
L- **Context splitting**: Split contexts to prevent unnecessary re-renders
L
L## LBundle Optimization
L### LCode Splitting
L- **Route-based splitting**: Split code at route boundaries
L- **Component lazy loading**: Lazy load non-critical components
L- **Dynamic imports**: Use dynamic imports for large libraries
L- **Vendor splitting**: Separate vendor code from application code
L
L### LBundle Analysis
L- **Regular analysis**: Analyze bundle size regularly
L- **Dependency auditing**: Audit and remove unused dependencies
L- **Tree shaking**: Ensure proper tree shaking configuration
L- **Compression**: Enable proper compression (gzip, brotli)
L
L## LAsset Optimization
L### LImage Optimization
L- **Modern formats**: Use WebP, AVIF when supported
L- **Responsive images**: Use srcset for different screen sizes
L- **Lazy loading**: Implement lazy loading for below-the-fold images
L- **Compression**: Optimize image compression settings
L
L### LFont Optimization
L- **Font subsetting**: Include only necessary character sets
L- **Font loading**: Use font-display: swap to prevent blocking
L- **Preloading**: Preload critical fonts
L- **Format selection**: Use WOFF2 with fallbacks
L
L## LNetwork Optimization
L### LHTTP/2 Optimization
L- **Resource multiplexing**: Take advantage of HTTP/2 multiplexing
L- **Server push**: Use server push for critical resources
L- **Header compression**: Leverage HPACK compression
L- **Connection reuse**: Maximize connection reuse
L
L### LCaching Strategy
L- **Cache headers**: Set appropriate Cache-Control headers
L- **Service workers**: Implement service workers for caching
L- **CDN usage**: Use CDN for global content delivery
L- **Cache invalidation**: Implement proper cache invalidation
L
L## LDatabase Optimization
L### LQuery Optimization
L- **Index usage**: Ensure proper database indexes
L- **Query efficiency**: Optimize database queries
L- **Connection pooling**: Use connection pooling effectively
L- **Result pagination**: Implement proper pagination for large datasets
L
L### LData Loading
L- **Lazy loading**: Load data only when needed
L- **Prefetching**: Prefetch likely needed data
L- **Caching**: Implement proper data caching strategies
L- **Compression**: Compress data transfers
L
L## LJavaScript Optimization
L### LRuntime Performance
L- **Algorithm complexity**: Choose efficient algorithms and data structures
L- **Memory management**: Avoid memory leaks and excessive memory usage
L- **Garbage collection**: Help garbage collector by cleaning up references
L- **Event loop optimization**: Avoid blocking the event loop
L
L### LBuild Optimization
L- **Minification**: Enable JavaScript minification
L- **Dead code elimination**: Remove unused code
L- **Module concatenation**: Concatenate modules efficiently
L- **Source maps**: Generate source maps for debugging
L
L## LCSS Optimization
L### LCritical CSS
L- **Above-the-fold**: Inline critical CSS
L- **Non-blocking**: Load non-critical CSS asynchronously
L- **CSS minimization**: Minify CSS output
L- **Unused CSS**: Remove unused CSS rules
L
L### LRendering Optimization
L- **Layout thrashing**: Avoid forced synchronous layouts
L- **Paint optimization**: Minimize expensive paint operations
L- **Composite layers**: Promote elements to their own layers when beneficial
L- **GPU acceleration**: Use CSS transforms for GPU acceleration
L
L## LMonitoring & Measurement
L### LPerformance Monitoring
L- **Real user monitoring**: Monitor real user performance
L- **Synthetic monitoring**: Use synthetic tests for consistent monitoring
L- **Performance budgets**: Set and monitor performance budgets
L- **Regression detection**: Detect performance regressions automatically
L
L### LMetrics Collection
L- **Core Web Vitals**: Monitor all Core Web Vitals metrics
L- **Custom metrics**: Define and monitor custom performance metrics
L- **User experience**: Monitor user experience metrics
L- **Business impact**: Connect performance to business metrics
L
L## LDevelopment Tools
L### LPerformance Profiling
L- **Browser DevTools**: Use browser developer tools for profiling
L- **React DevTools**: Use React DevTools Profiler
L- **Lighthouse**: Run regular Lighthouse audits
L- **Performance budgets**: Set up performance budget monitoring
L
L### LBuild Tools
L- **Bundle analyzer**: Use bundle analyzers to identify large dependencies
L- **Webpack Bundle Analyzer**: Analyze Webpack bundle composition
L- **Lighthouse CI**: Integrate Lighthouse into CI pipeline
L- **Performance budgets**: Set performance budgets in build tools
L
L## LProgressive Enhancement
L### LGraceful Degradation
L- **Feature detection**: Detect browser capabilities
L- **Fallback implementation**: Provide fallbacks for unsupported features
L- **Progressive loading**: Load features progressively
L- **Offline capability**: Implement offline functionality
L
L### LMobile Optimization
L- **Responsive design**: Ensure mobile-first responsive design
L- **Touch optimization**: Optimize for touch interactions
L- **Network awareness**: Adapt to network conditions
L- **Battery awareness**: Consider battery impact on mobile devices
L
L## LSecurity Performance
L### LSecure Performance
L- **HTTPS enforcement**: Ensure all resources load over HTTPS
L- **Security headers**: Implement security headers without performance cost
L- **CSP optimization**: Optimize Content Security Policy for performance
L- **Certificate optimization**: Optimize SSL/TLS handshake performance
L
L## LContinuous Optimization
L### LPerformance Culture
L- **Regular audits**: Conduct regular performance audits
L- **Team awareness**: Build performance awareness in the team
L- **Documentation**: Document performance guidelines and best practices
L- **Training**: Provide performance training and resources
L
L### LAutomation
L- **CI/CD integration**: Integrate performance checks in CI/CD
L- **Automated testing**: Automate performance regression testing
L- **Alerting**: Set up performance alerting and monitoring
L- **Optimization workflows**: Create workflows for performance optimization






