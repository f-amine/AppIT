# 🤖 OrchestrAI

Orchestrate AI workflows with seamless data integration. Automate web crawling, data extraction, and AI-ready pipelines.

_This repository is in active development. While functional, some modules are still being integrated into the mono repo._

## What is OrchestrAI?

OrchestrAI is an intelligent orchestration platform that crawls websites, extracts structured data, and transforms it into AI-ready pipelines. Automate complex workflows with built-in crawling, scraping, and LLM integration.

*Join our stargazers to stay updated! ⭐*.

---

### API Key
Get started at [OrchestrAI](https://orchestrai.framer.website/) for your API key. <!-- Update domain -->

---

## Features

### Core Capabilities
- **Orchestrate**: Build end-to-end AI workflows with crawling and data processing
- **Crawl**: Auto-discover and process website structures
- **Extract**: Transform content into schemas for RAG, fine-tuning, and analytics
- **Integrate**: Connect to vector DBs, LLMs, and automation tools

### Advanced Features
- **Workflow Automation**: Chain crawling, extraction, and AI tasks
- **Dynamic Execution**: Browser automation, retries, and JS rendering
- **Multi-Format Support**: Websites, PDFs, DOCX, and images
- **Enterprise Scalability**: Batch processing, proxies, and anti-bot handling

---

## Quickstart Examples

### Run a Workflow
```bash
curl -X POST https://api.orchestrai.dev/v1/run \  <!-- Update domain -->
    -H 'Authorization: Bearer oai-YOUR_API_KEY' \  <!-- Update API key prefix -->
    -d '{
      "workflow": "crawl-extract",
      "url": "https://docs.orchestrai.dev"
    }'
```

### Extract Structured Data
```python
from orchestrai import OrchestrAI  # Updated SDK

class ProductSchema(BaseModel):
    features: list[str]
    pricing: str

data = OrchestrAI(api_key="oai-YOUR_KEY").extract(
    url="https://orchestrai.dev/pricing",
    schema=ProductSchema
)
```

---

## SDK Installation

### Python
```bash
pip install orchestrai
```

### Node.js
```bash
npm install @orchestrai/sdk
```

---

## Deployment Options

OrchestrAI is open-source (AGPL-3.0) with a managed cloud service:

| Feature               | Self-Hosted | Cloud          |
|-----------------------|-------------|----------------|
| Workflow Automation   | ✅          | ✅ (Enhanced)  |
| Browser Execution     | ❌          | ✅             | 
| Enterprise SLAs       | ❌          | ✅             |
| Free Tier             | ✅          | ✅             |

---

## Contributing
We welcome contributions! See [CONTRIBUTING.md](CONTRIBUTING.md). 

**Note**: Users must respect website terms of service and robots.txt rules.

---

## License
- Core: AGPL-3.0
- SDKs: MIT

---

<p align="right">
  <a href="#readme-top">↑ Back to Top ↑</a>
</p>
