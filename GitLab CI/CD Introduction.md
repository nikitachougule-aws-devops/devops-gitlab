## GitLab CI/CD Introduction

**CI/CD** stands for:

- **CI** – Continuous Integration
- **CD** – Continuous Delivery / Continuous Deployment

CI/CD automates the process of building, testing, and deploying applications.

---

### Continuous Integration (CI)

Continuous Integration is the practice of automatically building and testing code whenever developers push changes to the repository.

---

### Continuous Delivery (CD)

Continuous Delivery automatically prepares the application for deployment after successful testing.

Deployment still requires **manual approval**.

---

### Continuous Deployment

Continuous Deployment automatically deploys the application to production after all tests pass.

No manual approval is required.

---

### CI/CD Workflow

```text
Developer
     │
     ▼
Write Code
     │
     ▼
Commit Changes
     │
     ▼
Push to GitLab
     │
     ▼
CI/CD Pipeline Starts
     │
     ▼
Build
     │
     ▼
Test
     │
     ▼
Deploy
```

---

### What is GitLab CI/CD?

- It is GitLab's built-in automation tool.
- It automatically: Builds applications, Runs tests, Deploys applications
- The pipeline is defined using a file called:

```text
.gitlab-ci.yml
```

---

### GitLab CI/CD Components

| Component | Purpose |
|-----------|---------|
| Pipeline | Complete automation workflow |
| Stage | Group of related jobs |
| Job | A single task in the pipeline |
| Runner | Executes jobs |
| `.gitlab-ci.yml` | Defines the pipeline |

---

### GitLab CI/CD Flow

```text
Git Push
    │
    ▼
GitLab
    │
    ▼
Read .gitlab-ci.yml
    │
    ▼
Create Pipeline
    │
    ▼
Runner Executes Jobs
    │
    ▼
Build
    │
    ▼
Test
    │
    ▼
Deploy
```

---

### Key Points

- **CI** automatically builds and tests code after every push.
- **Continuous Delivery** prepares the application for deployment with manual approval.
- **Continuous Deployment** automatically deploys the application after successful tests.
- GitLab CI/CD uses the `.gitlab-ci.yml` file to define pipelines.
- A pipeline consists of **stages**, **jobs**, and **runners**.
