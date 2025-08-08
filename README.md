# Employee Directory

## DESCRIPTION

### Goal
Build a minimal Python API framework that supports HTTP routing, middleware (logging, authentication), JSON response handling, and API versioning. This framework will be used to build an employee directory API for a high school, modeling real enterprise backend needs.

### Core Features
- Routing by HTTP method and path, including dynamic parameters (e.g., /employees/{id})
- Middleware support for logging requests and simple authentication
- Automatic JSON serialization of handler responses
- Standardized error handling with JSON responses
- Basic API versioning through URL prefixes (e.g., /v1/employees)

___

## TODO

### Phase 1: Planning & Setup
- [x] Write a brief design note (goal, core features, todo)
- [x] Create your GitHub repo, initialize with README and .gitignore
- [x] Add your mock employee data CSV/JSON into the repo or a data/ folder
- [x] Setup a basic Python project structure (myapi/, tests/, etc.)

### Phase 2: Minimal HTTP Server
- [ ] Build a very simple HTTP server using Python’s socket or http.server modules
- [ ] Respond to a fixed route /hello with a simple JSON message
- [ ] Setup basic request parsing for path and method
- [ ] Commit early and often (good commit messages!)

### Phase 3: Routing System
- [ ] Implement routing to map HTTP methods and paths (e.g., /employees, /employees/{id}) to handler functions
- [ ] Add support for path parameters (e.g., /employees/123)
- [ ] Test routing logic with a few dummy routes

### Phase 4: Middleware
- [ ] Add middleware capability (functions that run before/after handlers)
- [ ] Implement logging middleware to log each request (method, path, time)
- [ ] Add a simple auth middleware stub (e.g., check for a header X-API-Key) that can be extended later

### Phase 5: JSON Serialization & Response Handling
- [ ] Automatically serialize Python dicts/lists to JSON responses
- [ ] Standardize response structure with status codes and headers
- [ ] Implement error handling middleware to catch exceptions and return JSON error responses

### Phase 6: Implement Basic API Endpoints Using Your Framework
- [ ] Load your employee mock data into memory (e.g., list or dict)
- [ ] Implement these routes:
- [ ] GET /employees — return list of all employees
- [ ] GET /employees/{id} — return employee by ID or 404 if not found
- [ ] Optional: filtering by department query param (/employees?department=math)

### Phase 7: Testing & Documentation
- [ ] Write unit tests for routing, middleware, and API endpoints using pytest
- [ ] Add a clear README with:
- [ ] How to run the server
- [ ] Example API usage snippets
- [ ] Description of the middleware features
- [ ] Optional: Dockerize your app with a simple Dockerfile

### Phase 8: Bonus Features
- [ ] Add API versioning (support /v1/employees)
- [ ] Add request validation (check POST/PUT payloads against schema)
- [ ] Add persistence with SQLite for your employee data instead of in-memory
- [ ] Auto-generate API docs (Swagger/OpenAPI)

___

## USAGE

### To Set Up

### To Run

### To Test

___

## NOTES

### Commit Guide
| type | description |
| - | - |
| build | Changes that affect the build system or external dependencies |
| ci | Changes to our CI configuration files and scripts |
| docs | Documentation only changes |
| feat | A new feature |
| fix | A bug fix |
| perf | A code change that improves performance |
| refactor | A code change that neither fixes a bug nor adds a feature |
| style | Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc) |
| test | Adding missing tests or correcting existing tests |
