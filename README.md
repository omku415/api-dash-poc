# API Dash – OpenAPI Template Generator (PoC)

## Overview

This project is a Proof of Concept (PoC) for automating API integration workflows in API Dash.

It takes an OpenAPI specification (JSON) as input and generates ready-to-use API request templates. The goal is to reduce manual API setup and improve developer onboarding.

---

## Features

- OpenAPI parsing (paths, methods, parameters, request body)
- Data normalization into a consistent structure
- Automatic endpoint tagging (User, Weather, Finance, etc.)
- Metadata enrichment (base URL and authentication type)
- API template generation
- Express API endpoint: `POST /generate`
- Minimal UI for interactive testing

---

## How It Works

```
OpenAPI JSON → Parse → Normalize → Tag → Enrich → Generate Templates
```

---

## Live Demo

https://api-dash-poc.onrender.com

---

## Run Locally

```bash
npm install
npm start
```

Open in browser:

```
http://localhost:3000
```

---

## API Endpoint

### POST `/generate`

Request:
- OpenAPI JSON in the request body

Response:
- Generated API templates in JSON format

---

## Project Structure

```
src/
  parser/
  normalizer/
  tagger/
  generator/
  utils/
  routes/
  app.js

public/
  index.html

sample/
  sample-openapi.json
```

---

## Future Scope

- Integration with AI agents for dynamic API execution
- Interactive API UI rendering inside chat interfaces
- Schema-based request body generation
- Improved tagging and categorization logic

---

## Motivation

Setting up APIs manually is repetitive and time-consuming.

This PoC demonstrates how OpenAPI specifications can be transformed into structured request templates automatically, providing a foundation for intelligent API tooling and AI-assisted workflows.