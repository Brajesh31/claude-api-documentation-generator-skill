# claude-api-documentation-generator-skill

A Claude Code skill for generating and maintaining clear API documentation from an existing implementation or API specification.

## Overview

This skill helps transform routes, schemas, controllers, and service behavior into documentation that developers can use. It supports REST, GraphQL, and WebSocket APIs, with attention to endpoint descriptions, authentication, request and response formats, error handling, and examples.

Documentation should describe the actual API behavior, not an imagined or intended interface.

## Main Capabilities

- Inspect API routes and handlers.
- Identify endpoints and supported methods.
- Extract request parameters and schemas.
- Document authentication requirements.
- Describe response structures and status codes.
- Explain common error conditions.
- Create usage examples.
- Organize API reference material.
- Generate or update OpenAPI-style specifications where appropriate.
- Review documentation for consistency and completeness.

## When to Use It

Use this skill when creating API documentation, updating an existing reference, onboarding developers, preparing an API for external consumers, or producing a specification from a codebase.

## Installation

```bash
git clone https://github.com/Brajesh31/claude-api-documentation-generator-skill.git ~/.claude/skills/api-documentation-generator
```

## Usage

Invoke the skill for API documentation work:

```text
/api-documentation-generator
```

Provide the API repository, intended audience, output format, authentication model, and any existing schemas or examples.

## Recommended Workflow

1. Inspect the API structure and identify entry points.
2. Trace routes to their actual handlers and services.
3. Inspect validation schemas and middleware.
4. Identify authentication and authorization requirements.
5. Record request and response formats.
6. Document status codes and error behavior.
7. Create examples using valid representative values.
8. Generate or update the API specification.
9. Compare documentation against implementation.
10. Review for missing endpoints and outdated examples.

## Documentation Structure

A useful API reference commonly includes:

- Overview and base URL configuration.
- Authentication and authorization.
- Endpoint groups.
- Request parameters and schemas.
- Response schemas and examples.
- Error codes and troubleshooting.
- Pagination, filtering, and sorting.
- Rate limits and retry behavior.
- Versioning and deprecation.
- SDK or integration examples where available.

## Quality Checklist

- Every documented endpoint exists.
- Methods and paths match the implementation.
- Required parameters are identified.
- Authentication requirements are accurate.
- Response examples match actual schemas.
- Error codes are realistic.
- Sensitive values are not included.
- Examples can be followed without hidden assumptions.
- Version and deprecation status are clear.
- Documentation changes are reviewed alongside API changes.

## Repository Contents

- `SKILL.md`: Main API documentation workflow.
- `README.md`: Coverage, process, and documentation checklist.

## Practical Principle

Never invent an endpoint, parameter, or response field to make documentation look complete. If the implementation does not reveal the behavior, mark it as unknown and request confirmation.
