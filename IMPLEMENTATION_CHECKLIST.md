# Implementation Checklist

Build the application yourself using `PROJECT_BRIEF.md`.

## Initial setup

- [ ] Read the project specification.
- [ ] Review the architecture and data model.
- [ ] Create a Python virtual environment.
- [ ] Install and pin the required dependencies.
- [ ] Configure credentials through environment variables.
- [ ] Review the data privacy and security requirements.

## Project acceptance criteria

- [ ] Upload succeeds for files ≤5 MB
- [ ] Schema JSON returned within 2 s
- [ ] Supported formats: .csv, .xlsx
- [ ] Plan contains ≥3 actionable steps for a typical messy dataset
- [ ] Each step includes description, pandas code snippet, and confidence score
- [ ] Approved plan produces cleaned file without errors
- [ ] Execution time ≤5 s for 100 k rows
- [ ] Generated audit log lists original vs. transformed values
- [ ] DVC commit created for each run
- [ ] User can retrieve previous version via API
- [ ] Set up FastAPI project skeleton
- [ ] Implement secure file upload endpoint
- [ ] Add schema inference using pandas‑profiling
- [ ] Create LangChain prompt templates
- [ ] Integrate Groq/OpenAI API
- [ ] Generate cleaning plan JSON
- [ ] Store plan in PostgreSQL
- [ ] Build minimal Swagger UI for plan approval
- [ ] Sandbox pandas execution (subprocess with timeout)
- [ ] Persist cleaned file and DVC commit
- [ ] Design audit log schema
- [ ] Implement audit endpoint
- [ ] Write unit & integration tests (pytest)
- [ ] Dockerize application
- [ ] Create GitHub Actions workflow (lint, test, build)
- [ ] Deploy to Render/ Railway (free tier)
- [ ] Unit tests for each FastAPI endpoint (coverage ≥ 90%)
- [ ] Integration test that uploads a synthetic dirty CSV, runs full pipeline, and checks that audit log matches expected transformations
- [ ] Security test: verify uploaded files are scanned for malicious content (e.g., CSV injection) and size limits enforced
- [ ] Docker image built with multi‑stage Dockerfile
- [ ] Push to Docker Hub (private)
- [ ] Deploy on Railway with PostgreSQL addon and persistent volume for DVC repo
- [ ] Enable HTTPS via Railway’s automatic certs

## Before completion

- [ ] Implement the planned MVP features.
- [ ] Add unit and integration tests.
- [ ] Run the test suite.
- [ ] Measure the evaluation metrics in the brief.
- [ ] Record actual results and known limitations.
- [ ] Document setup and deployment.
- [ ] Update the README to reflect the implemented features.
- [ ] Add only verified outcomes to your resume.
