# MCP Nantua

MCP Nantua is the public API layer for services built around the **Barba‑CV ecosystem**.

It exposes developer‑friendly endpoints that allow applications, agents, and platforms to interact with CV processing services.

The project focuses on **API surface, integration examples, and developer documentation**.

The processing engine itself is not part of this repository.

---

# Relationship with Barba‑CV

MCP Nantua is built on top of the **Barba‑CV specification**.

Barba‑CV defines the **standard JSON format for CV data**, while MCP Nantua provides the **API gateway used to access services built around this format**.

Barba‑CV specification repository:

https://github.com/Eurobotics-Association/barba-cv

---

# What this repository contains

This repository provides:

* API documentation
* integration guides
* example requests
* SDK examples
* developer tutorials

It does **not contain the Barba‑CV engine implementation**.

---

# Example use cases

Applications may use MCP Nantua to:

* submit CVs for processing
* convert documents into Barba‑CV JSON
* validate CV data
* generate ATS‑compliant CV formats
* integrate CV automation into HR platforms

---

# Example API flow

Typical integration flow:

1. Client uploads a CV
2. API processes the request
3. CV is converted into Barba‑CV JSON
4. structured output is returned

Example request:

```
POST /api/cv/process
```

Example response:

```
{
  "status": "processing",
  "job_id": "abc123"
}
```

---

# Repository structure

```
mcp-nantua/

api/
  openapi.yaml

examples/
  curl/
  python/
  javascript/

sdk/
  js/
  python/

docs/
  integration.md
  quickstart.md

LICENSE
README.md
```

---

# License

This repository is released under the **MIT License**.

The goal is to maximize developer adoption and simplify reuse of documentation and examples.

---

# Important note

This repository documents the API surface only.

The internal processing engine and infrastructure are proprietary and maintained privately.

---

# Maintainer

MCP Nantua is developed and maintained by **LGB SAS**.

---

# Vision

MCP Nantua aims to make it simple for:

* developers
* HR platforms
* AI agents
* recruiting tools

to interact with services built on top of the **Barba‑CV standard**.
