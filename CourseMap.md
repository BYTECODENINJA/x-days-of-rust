# RUST PROGRAMMING WITH AXUM

## Projects to be built by the end
- [ ] A custom extractor that reads an API Key
- [ ] A custom response type for created resources
- [ ] A custom error type: one format for every failure
- [ ] A custom tower layer, written by hand
- [ ] A custom Rate limiter
- [ ] A custom websocket hub with rooms and prescence
- [ ] A custom upload pipeline, with file sniffing
- [ ] A custom resumable upload protocal
- [ ] A custom signed URL scheme

## PART 1: Foundations

### Module 1: Rust and HTTP essentials
   - Async / Await
   - Traits and generics
   - Closures
   - Arc & Mutex
   - Serde
   - Result and ?
   - URLs
   - Methods
   - status codes
   - HTTP Headers
   - REST
   - Using Curl
 
### Module 2: Handlers and First responses
- Async fn handlers
- String / &str
- HTML
- StatusCodes
- Turples
- Impl IntoResponse
- Redirects
- Health Check
 
### Module 3: Routing
- get, post, put, delete, patch
- {path} params
- wildcards
- nest, merge
- 404 / 405 fallbacks
- Trailling slashes
- serving services

### Module 4: Extractors
- Path, Query, Json, Form
- Headers, raw bytes
- client address
- what happens if they fail
- order matters: body last

### Module 5: Responses in depth
- IntoResponse
- ResponseParts
- Header turples
- streaming
- create response types

### Module 6: Shared State
- State extractor
- Locks vs Atomics
- Sub states
- Dependency injection
- Testing with fakes

### Module 7: Error handling
- Error enum
- thiserror
- anyhow
- ? inside handlers
- custom rejections
- panic catching
- JSON problem responses

### Module 8: Validattion and custom extractors
- Validator
- garde
- ValidatedJson
- Derive macros
- Body size limits
- read a body twice
 
By the end of this part, you'll have a solid foundation in Rust and HTTP, and be ready to move on to more advanced topics.You are able to create a CRUD app.

## PART 2: Middleware and Tower
### Module 9: Tower Fundamentals
- Service + Layer by hand
- Layer order rule
- layer Vs Route-layer
- timeouts
- Limits
- Load shedding
- one-shot router tests
### Module 10: Axum middleware
- from_fn
- map_request, map_response
- optional layers
- reading bodies
- Rate limiter Project
### Module 11: The tower-http toolbox
- requets tracing
- CORS
- Compresion
- Request ids
- body limits
- CSRF protection
- Header Validation
- Panic catching
- Path normalization
### Module 12: Static files and server-rndered HTML
- serve a folder
- SPA fallbacks
- files embedded + ETag
- Askama
- Minijinja
- Maud
- Post-Redirect-get
- HTMX
  
## PART 3: SQLx, Postgres, Redis
### Module 13: SQLx and Postgres
- connection pool
- embedded migrations
- typed queries
-  enums
- transactions
- compile-time checked SQL
- docker compose up
### Module 14: Architecture and the repository pattern
- handlers, services, repositories
- repository trait
- generics vs dyn
- contract test
- swap in-memory, postgres
  
### Module 15: ORMs and Other databases
- SQLx + SQLite
- SeaORM
- Diesel async
- tokio-postgress
- MongoDb
  
### Module 16: Caching and Rate limiting
- Redis
- in-process cache
- Etag + conditional requests
- rate limiter
- concurrency limits
- Graceful degredation
### Module 17: Rest API design
- pagination
- filtering
- sorting
- PATCH semantics
- Idempotency keys
- Versioning
- One error format
- typed routes

## PART 4: Auth and Security
### Module 18: Passwords and users
- Why we Hash
- argon2
- registration + login
- same-time failures
- account lockout
- reset tokens

### Module 19: JWT Authentication
- pinned algorithm
- Key rotation
- blacklist
- AuthUser extractor

### Module 20: Cookies and Sessions
- Cookie jar
- Signed cookies
- Private cookies
- tower sessions
- session fixation
- flash messages
- custom SQLx store

### Module 21: Authorization
- 401: Who are you
- 403: You may not
- 404: Pretend its not here
- Roles
- Permisions
- Guard Layers
- API Keys
- Ownership Checks
- Tenant scoping

### Module 22: Security Hardening
- Security headers + CSP
- Strict CORS list
- SQL injection
- SSRF
- Secrets Handling
- Self Audit
- Dependency Audit
## PART 5: Realtime, Uploads, Video Streaming
- WebSockets
- Server-Sent Events
- Streaming bodies
- Uploads and downloads
- Chunked and resumable uploads
- Range requests and Chunked downloads
- Streaming Video and audio
- Background jobs and messaging
- Calling other services and proxying
## PART 6: API Styles, OpenAPI, GraphQL, gRPC
## PART 7: Testing, Tracing, Perfomance, TLS, Docker
## PART 8: Deployment, CI/CD, Monitoring, Logging
## CAPSTONE PROJECTS