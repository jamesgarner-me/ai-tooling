# Rules

## General

## Language & Style
- Use British English for all text and documentation
- Don't use placeholders like `// ... rest of the processing ...` in code examples
- Provide complete implementations without omissions
- Break problems into smaller steps and think through each step separately

## Documentation & Testing
- Always review contents of /memory-bank folder for context
- Document changes clearly in progress.md
- Unit tests should be updated when making code changes
- Provide a PLAN with REASONING before making changes
- Explain OBSERVATIONS and REASONING when diagnosing issues

## Design Principles
- UI should be responsive and accessible
- Modal components should not cause scrollbars to appear
- GIFs and images should be properly sized for different screen sizes
- Use proper ARIA attributes for accessibility 

## Project Specific 

## Frontend Conventions
- React components use TypeScript with .tsx extension
- Component files follow PascalCase naming convention
- CSS is imported directly into component files
- Vite is used as the build tool with environment-specific configurations
- Base path for production is set to /example-app-base-route/
- Static assets are imported directly
- UI components are located in src/components/ui/
- Context providers are used for state management

## Backend Conventions
- Python with FastAPI for the backend API
- Use proper CORS configuration including origin regex patterns
- Lambda functions are deployed to AWS
- Using Mangum to adapt FastAPI to AWS Lambda

## AWS & Infrastructure
- CloudFormation is used for infrastructure as code
- Lambda@Edge functions must be created in us-east-1 region
- CloudFront is used for content delivery
- S3 is used for static asset storage
- API Gateway is used for API endpoints
- Route 53 is used for DNS management
- Certificate Manager is used for SSL certificates
- Path patterns in CloudFront must be properly configured for both with and without trailing slashes

## Deployment
- GitHub Actions is used for CI/CD
- Frontend and backend have separate deployment workflows
- Cache settings are carefully configured for different types of assets
- Error pages are configured for appropriate response codes