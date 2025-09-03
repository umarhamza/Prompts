# Project Technology & Structure Audit (match house style)

**Goal**
Inventory the technologies and structure of the codebase at `{REPO_PATH}`, matching our concise internal documentation style. Focus on listing all discoverable features and capabilities.

**Inputs**
* Repository path: `{REPO_PATH}`
* Scope hint: `{SCOPE_NOTE}` (optional)

**Rules (house style)**
* Don't include product-manager sections (no success criteria, timelines, migrations)
* Don't write any code in the document
* Ask up to **5** clarifying questions only if the repo structure is unclear; otherwise proceed
* Be concise and precise
* State only what's evidenced in files; mark unknowns clearly

**What to produce**
A single markdown document saved to **`docs/PROJECT_AUDIT.md`** containing:

### 1. **Overview** (2–3 sentences)
Brief description of what the project does and its primary purpose.

### 2. **Technology Stack**
* **Languages/runtimes** (with versions if discoverable)
* **Frameworks/libraries** (frontend, backend, mobile)
* **Package managers & build tools**

### 3. **Architecture & Modules**
* **App type** (monolith/microservices; SPA/SSR/CSR; API style)
* **Layers/modules** and their responsibilities
* **Communication patterns** (REST, GraphQL, gRPC, etc.)

### 4. **Project Structure (tree)**
* **Directory tree** (depth 2–3) highlighting key folders
* **Entry points** & routing approach
* **Workspaces/monorepo** notes if applicable

### 5. **Features & Capabilities**
List all discoverable features by examining:
* Route definitions and API endpoints
* Component/module exports
* Database schemas and models
* Configuration files
* Documentation and README files
* Test files (feature descriptions)

Group features by:
* **Core Features** (primary functionality)
* **User Features** (user-facing capabilities)
* **Admin Features** (administrative functionality)
* **API Features** (programmatic interfaces)
* **Integration Features** (external service connections)

### 6. **Data Layer**
* **Databases** (type, schema insights)
* **ORMs/migrations** approach
* **Caching/queues/search** implementations
* **Data models** and relationships

### 7. **Auth & Security**
* **Authentication** approach (JWT, OAuth, sessions)
* **Authorization** (roles, permissions, middleware)
* **Security measures** (CORS, rate limiting, validation)
* **Secrets management**

### 8. **Tooling & Quality**
* **Test frameworks** and coverage approach
* **Linters/formatters** configuration
* **CI/CD** pipelines and deployment targets
* **Development tools** and scripts

### 9. **Config & Environments**
* **Environment variables** and configuration files
* **Environment conventions** (dev/staging/prod)
* **Feature flags** or toggles

### 10. **Integrations**
* **External APIs** and SDKs
* **Webhooks** and event handling
* **Third-party services** (payment, email, storage, etc.)

### 11. **Local Quickstart**
* **Setup commands** (quote exact scripts from package.json, Makefile, etc.)
* **Run commands** for development
* **Test commands** and verification steps

### 12. **Evidence (file paths)**
For each section, bullet the specific files inspected:
* *`package.json`*, *`requirements.txt`*, *`Gemfile`*, *`go.mod`*
* *`docker-compose.yml`*, *`Dockerfile`*
* *`.env.example`*, *`config/`*, *`appsettings.*.json`*
* *`src/routes/`*, *`controllers/`*, *`models/`*
* *`README.md`*, *`docs/`*
* Test files and configuration

### 13. **Risks, Gaps & Follow-ups**
* **Red flags** (security concerns, deprecated dependencies)
* **Missing pieces** (documentation, tests, error handling)
* **Next checks** (areas needing deeper investigation)
* **Unknown features** (areas that need manual verification)

**Constraints**
* Use British spelling throughout
* Keep bullets tight and informative
* Mark uncertainties clearly with "Unknown:" or "To verify:"
* If codebase is very large, may add **Phases** for systematic review

