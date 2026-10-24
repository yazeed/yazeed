L# LSecurity & Reliability Rules
L
L## LSecurity Philosophy
L- **Defense in depth**: Implement multiple layers of security
L- **Fail-safe defaults**: Default to secure configurations
L- **Principle of least privilege**: Grant minimal necessary permissions
L- **Zero trust**: Never trust, always verify
L
L## LAuthentication & Authorization
L### LAuthentication Security
L- **Password policies**: Enforce strong password requirements
L- **Multi-factor authentication**: Require MFA for sensitive operations
L- **Session management**: Implement secure session handling
L- **Token security**: Use secure token generation and storage
L
L### LAuthorization Controls
L- **Role-based access**: Implement proper role-based permissions
L- **Resource ownership**: Validate resource ownership for operations
L- **API authorization**: Secure all API endpoints with proper authorization
L- **Permission inheritance**: Handle permission inheritance correctly
L
L## LData Protection
L### LInput Validation
L- **Server-side validation**: Never trust client-side validation alone
L- **Input sanitization**: Sanitize all user inputs
L- **Type validation**: Validate data types and structure
L- **Length limits**: Enforce reasonable input length limits
L
L### LData Storage
L- **Encryption at rest**: Encrypt sensitive data in databases
L- **Secure key management**: Properly manage encryption keys
L- **Data classification**: Classify data by sensitivity level
L- **Retention policies**: Implement data retention and deletion policies
L
L## LNetwork Security
L### LHTTPS Implementation
L- **SSL/TLS enforcement**: Require HTTPS for all connections
L- **Certificate management**: Properly manage SSL certificates
L- **HSTS headers**: Implement HTTP Strict Transport Security
L- **Certificate pinning**: Consider certificate pinning for APIs
L
L### LAPI Security
L- **Rate limiting**: Implement rate limiting to prevent abuse
L- **Request validation**: Validate all API requests
L- **CORS configuration**: Properly configure CORS policies
L- **API versioning**: Use proper API versioning strategies
L
L## LFrontend Security
L### LXSS Prevention
L- **Content escaping**: Properly escape user-generated content
L- **CSP headers**: Implement Content Security Policy
L- **Sanitized rendering**: Use safe rendering methods
L- **Input validation**: Validate and sanitize all inputs
L
L### LCSRF Protection
L- **Token validation**: Use CSRF tokens for state-changing operations
L- **SameSite cookies**: Configure cookies with SameSite protection
L- **Origin validation**: Validate request origins
L- **State validation**: Validate form state integrity
L
L## LDatabase Security
L### LAccess Controls
L- **Row Level Security**: Implement RLS in Supabase
L- **Parameterized queries**: Use parameterized queries to prevent SQL injection
L- **Connection limits**: Limit database connections per user
L- **Query timeouts**: Implement query execution timeouts
L
L### LData Integrity
L- **Foreign key constraints**: Use proper foreign key relationships
L- **Transaction management**: Use transactions for data consistency
L- **Backup verification**: Regularly verify backup integrity
L- **Audit logging**: Log all data modification operations
L
L## LInfrastructure Security
L### LEnvironment Security
L- **Secret management**: Use proper secret management (no hardcoded secrets)
L- **Environment isolation**: Isolate development, staging, and production
L- **Access controls**: Implement least privilege for infrastructure access
L- **Monitoring**: Monitor infrastructure for security events
L
L### LDeployment Security
L- **Secure pipelines**: Use secure CI/CD pipelines
L- **Code signing**: Sign releases and deployments
L- **Vulnerability scanning**: Scan for vulnerabilities in dependencies
L- **Container security**: Secure container configurations
L
L## LReliability Engineering
L### LError Handling
L- **Graceful degradation**: Handle errors gracefully without system failure
L- **Error boundaries**: Implement error boundaries in React applications
L- **Fallback UI**: Provide fallback UI for error states
L- **Error logging**: Log errors with proper context and severity
L
L### LResilience Patterns
L- **Circuit breakers**: Implement circuit breaker patterns
L- **Retry logic**: Implement intelligent retry mechanisms
L- **Timeout handling**: Set appropriate timeouts for operations
L- **Backoff strategies**: Use exponential backoff for retries
L
L## LMonitoring & Alerting
L### LApplication Monitoring
L- **Error tracking**: Implement comprehensive error tracking
L- **Performance monitoring**: Monitor application performance metrics
L- **User experience**: Track user experience metrics
L- **Business metrics**: Monitor business-critical metrics
L
L### LInfrastructure Monitoring
L- **System health**: Monitor system resource usage
L- **Service availability**: Monitor service uptime and availability
L- **Dependency health**: Monitor external dependency health
L- **Security events**: Monitor for security-related events
L
L## LIncident Response
L### LIncident Detection
L- **Automated alerts**: Set up automated alerting for critical issues
L- **Threshold monitoring**: Monitor for abnormal behavior patterns
L- **User reports**: Monitor user-reported issues
L- **Log analysis**: Analyze logs for potential issues
L
L### LResponse Procedures
L- **Escalation paths**: Define clear incident escalation procedures
L- **Communication plans**: Plan communication during incidents
L- **Recovery procedures**: Document system recovery procedures
L- **Post-mortem analysis**: Conduct thorough post-mortem analysis
L
L## LCompliance & Audit
L### LRegulatory Compliance
L- **Data protection**: Comply with data protection regulations (GDPR, CCPA)
L- **Industry standards**: Follow relevant industry security standards
L- **Privacy policies**: Implement proper privacy policies
L- **Consent management**: Manage user consent properly
L
L### LAudit Trails
L- **Activity logging**: Log all user and system activities
L- **Change tracking**: Track all configuration and code changes
L- **Access logging**: Log all access to sensitive resources
L- **Compliance reporting**: Generate compliance reports as needed
L
L## LCode Security
L### LSecure Coding Practices
L- **Input validation**: Validate all inputs thoroughly
L- **Output encoding**: Properly encode all outputs
L- **Secure defaults**: Use secure defaults in all configurations
L- **Least privilege**: Implement least privilege in code
L
L### LDependency Security
L- **Vulnerability scanning**: Regularly scan for vulnerabilities
L- **Dependency updates**: Keep dependencies updated and secure
L- **License compliance**: Ensure dependency licenses are acceptable
L- **Supply chain security**: Verify dependency supply chain integrity
L
L## LTesting Security
L### LSecurity Testing
L- **Penetration testing**: Conduct regular penetration testing
L- **Vulnerability scanning**: Scan for common vulnerabilities
L- **Code review security**: Include security in code review checklists
L- **Dependency auditing**: Audit third-party dependencies
L
L### LReliability Testing
L- **Load testing**: Test system performance under load
L- **Chaos engineering**: Test system resilience through chaos experiments
L- **Failover testing**: Test system failover capabilities
L- **Disaster recovery**: Test disaster recovery procedures
L
L## LContinuous Security
L### LSecurity Culture
L- **Team training**: Provide regular security training
L- **Security champions**: Appoint security champions in teams
L- **Security reviews**: Include security in all project reviews
L- **Threat modeling**: Conduct threat modeling for new features
L
L### LSecurity Automation
L- **Automated scanning**: Automate security vulnerability scanning
L- **Policy enforcement**: Automate security policy enforcement
L- **Compliance monitoring**: Automate compliance monitoring
L- **Security testing**: Integrate security testing in CI/CD
L
L## LThird-Party Risk
L### LVendor Assessment
L- **Security assessments**: Assess third-party vendor security
L- **Contract clauses**: Include security requirements in contracts
L- **Monitoring**: Monitor third-party service security
L- **Incident response**: Coordinate incident response with vendors
L
L### LIntegration Security
L- **Secure integrations**: Secure all third-party integrations
L- **API security**: Secure API integrations with proper authentication
L- **Data sharing**: Securely handle data shared with third parties
L- **Audit logging**: Log all third-party interactions






