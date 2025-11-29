# Sample API Project - Dummy JSON API

This is a sample API project based on Beeceptor Dummy JSON API for testing schema discovery and validation features.

## Base URL
`https://dummy-json.mock.beeceptor.com`

## API Endpoints

### GET /posts
List all available blog posts

### GET /posts/{post_id}
Retrieve a post by passing an integer ID

### GET /comments
Listing all the blog comments

### GET /countries
List of all countries with name and code

### GET /continents
List of all the continents on the earth with area, population, countries, lines, etc.

### PUT /projects/{project_id}
Update an existing project with new configuration

### PUT /repos/{owner}/{repo}/subscription
Set the subscription status for a repository

## Structure

- `schema/` - JSON Schema definitions for request, response, and error
- `example/` - Example JSON responses for different HTTP status codes
- `paths/` - API path definitions
- `traits/` - Reusable traits
- `components/` - Shared components

## Usage

This project can be used to test:
- Schema discovery from Git repositories
- Response validation against discovered schemas
- Coverage calculation based on schema rules
- Test execution with schema validation

## Testing

Use the base URL `https://dummy-json.mock.beeceptor.com` to test all endpoints.
