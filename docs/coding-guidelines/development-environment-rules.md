L# LDevelopment Environment & Tooling Rules
L
L## LEnvironment Philosophy
L- **Consistency first**: Ensure all developers have identical environments
L- **Automation priority**: Automate environment setup and maintenance
L- **Documentation driven**: Document all environment requirements
L- **Version pinning**: Pin all tool and dependency versions
L
L## LDevelopment Environment Setup
L### LSystem Requirements
L- **OS compatibility**: Support macOS, Windows, and Linux
L- **Hardware requirements**: Document minimum hardware requirements
L- **Network access**: Specify required network access and ports
L- **Security policies**: Adhere to corporate security policies
L
L### LTool Installation
L- **Version management**: Use version managers for runtime tools
L- **Package managers**: Use consistent package manager across platforms
L- **Path configuration**: Configure system PATH correctly
L- **Permission setup**: Set up proper file permissions
L
L## LBun Package Manager
L### LConfiguration
L- **Global installation**: Install bun globally for all developers
L- **Version consistency**: Ensure all developers use the same bun version
L- **Lockfile management**: Never commit incorrect lockfiles
L- **Dependency resolution**: Understand bun's dependency resolution
L
L### LWorkflow Integration
L- **Script execution**: Use bun run for all npm script execution
L- **Fast refresh**: Leverage bun's fast development server
L- **Type checking**: Use bun's built-in TypeScript checking
L- **Hot reload**: Take advantage of bun's fast hot reload
L
L## LIDE Configuration
L### LEditor setup
L- **Extension consistency**: Ensure all developers use the same extensions
L- **Settings synchronization**: Synchronize IDE settings across team
L- **Keyboard shortcuts**: Standardize keyboard shortcuts
L- **Theme consistency**: Use consistent color schemes
L
L### LTypeScript Configuration
L- **Strict mode**: Enable all strict TypeScript options
L- **Path mapping**: Configure proper TypeScript path mapping
L- **Declaration generation**: Generate type declarations appropriately
L- **Build optimization**: Optimize TypeScript compilation settings
L
L## LVersion Control
L### LGit Configuration
L- **Global config**: Set up consistent git configuration
L- **Ignore files**: Maintain comprehensive .gitignore files
L- **Hooks setup**: Set up pre-commit and pre-push hooks
L- **Branch naming**: Establish branch naming conventions
L
L### LGit Workflow
L- **Branch strategy**: Use consistent branching strategy
L- **Commit standards**: Enforce commit message standards
L- **Merge strategy**: Use consistent merge/rebase strategies
L- **Conflict resolution**: Establish conflict resolution procedures
L
L## LTesting Environment
L### LTest Setup
L- **Test runners**: Configure consistent test runners
L- **Test frameworks**: Use consistent testing frameworks
L- **Mock libraries**: Standardize mocking libraries
L- **Test utilities**: Create shared test utilities
L
L### LTest Execution
L- **Parallel execution**: Configure parallel test execution
L- **Coverage reporting**: Set up consistent coverage reporting
L- **CI integration**: Integrate with CI/CD pipelines
L- **Performance monitoring**: Monitor test execution performance
L
L## LBuild Tools
L### LVite Configuration
L- **Development server**: Configure development server properly
L- **Build optimization**: Optimize production builds
L- **Asset handling**: Configure proper asset handling
L- **Plugin management**: Manage Vite plugins consistently
L
L### LBuild Scripts
L- **Script naming**: Use consistent script naming conventions
L- **Cross-platform**: Ensure scripts work across platforms
L- **Error handling**: Implement proper error handling in scripts
L- **Performance**: Optimize build script performance
L
L## LDatabase Development
L### LLocal Database Setup
L- **Database versions**: Use consistent database versions
L- **Schema management**: Implement proper schema versioning
L- **Seed data**: Provide consistent seed data for development
L- **Migration handling**: Handle database migrations properly
L
L### LDatabase Tools
L- **GUI tools**: Recommend consistent database GUI tools
L- **CLI tools**: Standardize command-line database tools
L- **Backup procedures**: Implement proper backup procedures
L- **Data privacy**: Handle sensitive data appropriately
L
L## LAPI Development
L### LAPI Testing Tools
L- **REST clients**: Recommend consistent API testing tools
L- **GraphQL clients**: Use appropriate GraphQL testing tools
L- **Authentication**: Handle API authentication consistently
L- **Documentation**: Maintain API documentation
L
L### LMock Services
L- **Mock servers**: Set up consistent mock services
L- **Data generation**: Generate realistic mock data
L- **Contract testing**: Implement API contract testing
L- **Service virtualization**: Use service virtualization appropriately
L
L## LContainerization
L### LDocker Setup
L- **Image consistency**: Use consistent base images
L- **Development containers**: Set up development containers
L- **Multi-stage builds**: Implement efficient multi-stage builds
L- **Security scanning**: Scan container images for vulnerabilities
L
L### LContainer Orchestration
L- **Local development**: Set up local container orchestration
L- **Service discovery**: Implement proper service discovery
L- **Networking**: Configure container networking properly
L- **Volume management**: Handle data persistence in containers
L
L## LCloud Development
L### LLocal Cloud Simulation
L- **LocalStack**: Use LocalStack for AWS development
L- **MinIO**: Use MinIO for S3-compatible storage
L- **Cloud development kits**: Use appropriate cloud development tools
L- **Cost monitoring**: Monitor cloud development costs
L
L### LDeployment Tools
L- **Infrastructure as Code**: Use IaC tools consistently
L- **Deployment automation**: Automate deployment processes
L- **Environment parity**: Maintain environment parity
L- **Rollback procedures**: Implement rollback procedures
L
L## LSecurity Tools
L### LDevelopment Security
L- **Vulnerability scanning**: Integrate vulnerability scanning
L- **Secret management**: Handle secrets securely in development
L- **Code analysis**: Use static analysis security tools
L- **Dependency checking**: Check dependencies for vulnerabilities
L
L### LAuthentication Tools
L- **Local authentication**: Set up local authentication services
L- **Token management**: Handle authentication tokens securely
L- **Session management**: Manage development sessions properly
L- **Multi-factor auth**: Implement MFA in development
L
L## LMonitoring & Debugging
L### LDevelopment Monitoring
L- **Application logging**: Configure consistent logging
L- **Error tracking**: Set up error tracking in development
L- **Performance monitoring**: Monitor performance in development
L- **Health checks**: Implement health check endpoints
L
L### LDebugging Tools
L- **Browser dev tools**: Use browser developer tools effectively
L- **Debugger configuration**: Configure debuggers properly
L- **Profiling tools**: Use appropriate profiling tools
L- **Memory analysis**: Monitor memory usage and leaks
L
L## LCollaboration Tools
L### LCommunication
L- **Team chat**: Use consistent team communication tools
L- **Video conferencing**: Standardize video conferencing tools
L- **Screen sharing**: Use appropriate screen sharing tools
L- **Documentation**: Maintain shared documentation platforms
L
L### LProject Management
L- **Issue tracking**: Use consistent issue tracking systems
L- **Project boards**: Maintain project boards consistently
L- **Time tracking**: Implement time tracking if required
L- **Reporting**: Generate consistent project reports
L
L## LEnvironment Maintenance
L### LRegular Updates
L- **Dependency updates**: Keep dependencies updated regularly
L- **Security patches**: Apply security patches promptly
L- **Tool updates**: Update development tools regularly
L- **Documentation updates**: Keep environment documentation current
L
L### LEnvironment Monitoring
L- **Health checks**: Monitor development environment health
L- **Performance monitoring**: Monitor environment performance
L- **Resource usage**: Track resource usage and costs
L- **Incident response**: Have incident response procedures
L
L## LOnboarding & Training
L### LNew Developer Setup
L- **Automated setup**: Provide automated environment setup scripts
L- **Documentation**: Maintain comprehensive setup documentation
L- **Mentorship**: Provide mentorship for new developers
L- **Training materials**: Create training materials and guides
L
L### LKnowledge Sharing
L- **Internal wikis**: Maintain internal knowledge bases
L- **Code reviews**: Use code reviews for knowledge sharing
L- **Tech talks**: Organize regular technical presentations
L- **Documentation**: Encourage documentation contributions
L
L## LContinuous Integration
L### LLocal CI
L- **Pre-commit hooks**: Implement comprehensive pre-commit hooks
L- **Pre-push validation**: Validate code before pushing
L- **Automated testing**: Run tests automatically on changes
L- **Code quality checks**: Enforce code quality standards
L
L### LCI/CD Integration
L- **Pipeline consistency**: Maintain consistent CI/CD pipelines
L- **Environment parity**: Ensure CI/CD matches local environments
L- **Artifact management**: Handle build artifacts properly
L- **Deployment automation**: Automate deployment from CI/CD
L
L## LBackup & Recovery
L### LData Backup
L- **Regular backups**: Implement regular data backups
L- **Backup verification**: Verify backup integrity regularly
L- **Recovery testing**: Test recovery procedures regularly
L- **Retention policies**: Implement appropriate retention policies
L
L### LEnvironment Recovery
L- **Disaster recovery**: Have disaster recovery procedures
L- **Environment recreation**: Be able to recreate environments quickly
L- **Configuration backup**: Backup all configuration files
L- **Documentation**: Document recovery procedures thoroughly

