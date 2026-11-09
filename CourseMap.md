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
 - Module 1: Rust and HTTP essentials
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
 - Module 2: Handlers and First responses
    - Async fn handlers
    - String / &str
    - HTML
    - StatusCodes
    - Turples
    - Impl IntoResponse
    - Redirects
    - Health Check
 - Module 3: Routing
    - get, post, put, delete, patch
    - {path} params
    - wildcards
    - nest, merge
    - 404 / 405 fallbacks
    - Trailling slashes
    - serving services
 - Module 4: Extractors
    - Path, Query, Json, Form
    - Headers, raw bytes
    - client address
    - what happens if they fail
    - order matters: body last
 - Module 5: Responses in depth
    - IntoResponse
    - ResponseParts
    - Header turples
    - streaming
    - create response types
 - Module 6: Shared State
    - State extractor
    - Locks vs Atomics
    - Sub states
    - Dependency injection
    - Testing with fakes
 - Module 7: Error handling
    - Error enum
    - thiserror
    - anyhow
    - ? inside handlers
    - custom rejections
    - panic catching
    - JSON problem responses
 - Module 8: Validattion and custom extractors
    - Validator
    - garde
    - ValidatedJson
    - Derive macros
    - Body size limits
    - read a body twice
 
By the end of this part, you'll have a solid foundation in Rust and HTTP, and be ready to move on to more advanced topics.You are able to create a CRUD app.

## PART 2: Middleware and Tower
- Tower Fundamentals
    - Service + Layer by hand
    - Layer order rule
    - layer Vs Route-layer
    - timeouts
    - Limits
    - Load shedding
    - one-shot router tests
- Axum middleware
    - from_fn
    - map_request, map_response
    - optional layers
    - reading bodies
    - Rate limiter Project
- The tower-http toolbox
    - requets tracing
    - CORS
    - Compresion
    - Request ids
    - body limits
    - CSRF protection
    - Header Validation
    - Panic catching
    - Path normalization
- Static files and server-rndered HTML
    - serve a folder
    - SPA fallbacks
    - files embedded + ETag
    - Askama
    - Minijinja
    - Maud
    - Post-Redirect-get
    - HTMX
## PART 3: SQLx, Postgres, Redis
## PART 4: Auth and Security
## PART 5: Realtime, Uploads, Video Streaming
## PART 6: API Styles, OpenAPI, GraphQL, gRPC
## PART 7: Testing, Tracing, Perfomance, TLS, Docker
## PART 8: Deployment, CI/CD, Monitoring, Logging
## CAPSTONE PROJECTS