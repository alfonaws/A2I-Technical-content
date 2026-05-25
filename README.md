# AWS Agentic AI Incubator Program — Technical Use Cases

> **Production-Ready Agentic AI Architectures for SI Partners**  
> Amazon Web Services | 2026

---

## About This Repository

This repository contains the technical reference material for the AWS Agentic AI Incubator Program (Wave 2). Each use case document includes:

- **Market opportunity** and quantified economics
- **Reference architectures** with embedded diagrams from official AWS repos
- **Progressive deployment models** — from observer to fully autonomous
- **Code accelerators** — links to working GitHub samples you can fork and deploy
- **Customer success stories** with validated metrics
- **Key Performance Indicators** and competitive positioning

Start with the use case table below, then dive into individual documents for full technical detail.

---

## Use Cases

| # | Use Case | Key Metric | Repeatability | Time-to-Production |
|---|----------|-----------|---------------|-------------------|
| 1 | [Customer Service Agents](docs/04-customer-service-agents.md) | $80B global savings by 2026 | 60-70% | 3-8 weeks |
| 2 | [IT Operations & Ticket Resolution](docs/05-it-operations.md) | 256% ROI (Forrester validated) | 65-70% | 4-8 weeks |
| 3 | [Intelligent Document Processing](docs/06-document-processing.md) | 33-35% CAGR, highest repeatability | 65-75% | 4-8 weeks |
| 4 | [Sales Operations & Revenue](docs/07-sales-operations.md) | 2.6x commercial growth likelihood | 60-70% | 6-10 weeks |
| 5 | [Supply Chain & Procurement](docs/08-supply-chain.md) | Up to $180M savings per deployment | 60-70% | 8-12 weeks |
| 6 | [Software Development (Bonus)](docs/09-software-development.md) | 24% scaled adoption, highest of any AI use case | 55-65% | 1-12 weeks |

---

## Prioritization

```
Phase 1 (Immediate)     → Customer Service + IT Operations
Phase 2 (30-60 days)    → Document Processing + Sales Operations  
Phase 3 (Scale)         → Supply Chain & Procurement
```

---

## Platform Stack

All use cases are built on the same AWS platform foundation:

```
┌───────────────────────────────────────────────────────────────┐
│                  Amazon Bedrock AgentCore                      │
│  ┌────────────┐  ┌──────────┐  ┌────────┐  ┌─────────────┐  │
│  │  Identity   │  │  Memory  │  │ Tools  │  │Observability│  │
│  │  & Access   │  │(Session) │  │(Actions│  │ & Tracing   │  │
│  └────────────┘  └──────────┘  └────────┘  └─────────────┘  │
├───────────────────────────────────────────────────────────────┤
│                      Amazon Bedrock                            │
│  ┌─────────────┐  ┌────────────┐  ┌───────────────────────┐  │
│  │ Foundation   │  │ Knowledge  │  │      Guardrails       │  │
│  │ Models       │  │ Bases (RAG)│  │(Safety/PII/Grounding) │  │
│  │(Multi-model) │  │            │  │                       │  │
│  └─────────────┘  └────────────┘  └───────────────────────┘  │
├───────────────────────────────────────────────────────────────┤
│         Open Standards: MCP + A2A Protocols                   │
├───────────────────────────────────────────────────────────────┤
│  Frameworks: LangGraph │ CrewAI │ LlamaIndex │ Strands SDK   │
└───────────────────────────────────────────────────────────────┘
```

---

## Key Repositories

| Repository | Description | Link |
|-----------|-------------|------|
| Bedrock Agent Samples | Multi-agent patterns, action groups, knowledge bases | [awslabs/amazon-bedrock-agent-samples](https://github.com/awslabs/amazon-bedrock-agent-samples) |
| AgentCore Samples (Use Cases) | SRE Agent, Incident Response, AWS Ops Agent, DB Analyzer | [awslabs/agentcore-samples](https://github.com/awslabs/agentcore-samples) |
| Multi-Agent Collaboration Workshop | Supervisor-worker topology patterns | [aws-samples/bedrock-multi-agents-collaboration-workshop](https://github.com/aws-samples/bedrock-multi-agents-collaboration-workshop) |
| Multi-Agent with Strands | Event-driven orchestration + dynamic agent fabrication | [aws-samples/sample-multi-agent-collaboration-with-strands](https://github.com/aws-samples/sample-multi-agent-collaboration-with-strands) |
| AgentCore Prototype-to-Production | 8-lab workshop: local agent → enterprise deployment | [aws-samples/sample-amazon-bedrock-agentcore-prototype-to-production](https://github.com/aws-samples/sample-amazon-bedrock-agentcore-prototype-to-production) |
| AgentCore Fullstack Webapp | One-command deployable AI agent web app | [aws-samples/sample-amazon-bedrock-agentcore-fullstack-webapp](https://github.com/aws-samples/sample-amazon-bedrock-agentcore-fullstack-webapp) |
| IDP Pipeline | Intelligent Document Processing with hybrid search | [aws-samples/sample-aws-idp-pipeline](https://github.com/aws-samples/sample-aws-idp-pipeline) |
| IDP with Bedrock | CDK-based IDP, no training required | [aws-samples/intelligent-document-processing-with-amazon-bedrock](https://github.com/aws-samples/intelligent-document-processing-with-amazon-bedrock) |
| Agentic IDP | Multi-pattern: agentic orchestration + prompt flow | [aws-samples/aws-ai-intelligent-document-processing](https://github.com/aws-samples/aws-ai-intelligent-document-processing) |
| Sales Assistant (Vespa + AgentCore) | Hybrid search sales agent with streaming | [aws-samples/sample-bedrock-agentcore-vespa-ai-sales-assistant](https://github.com/aws-samples/sample-bedrock-agentcore-vespa-ai-sales-assistant) |
| Retail Agent | ReAct framework agent for customer interactions | [aws-samples/agentsforbedrock-retailagent](https://github.com/aws-samples/agentsforbedrock-retailagent) |
| AI-Powered SDLC | AI across all 6 software development lifecycle phases | [aws-samples/sample-ai-powered-sdlc-patterns-with-aws](https://github.com/aws-samples/sample-ai-powered-sdlc-patterns-with-aws) |
| Industry Use Cases | Vertical templates (auto, energy, FSI, healthcare, travel) | [aws-samples/amazon-bedrock-industry-use-cases](https://github.com/aws-samples/amazon-bedrock-industry-use-cases) |
| Kiro | Agentic IDE — spec-driven development, open source | [kirodotdev/Kiro](https://github.com/kirodotdev/Kiro) |

---

## Additional AWS Products (New 2026)

| Product | Description | Link |
|---------|-------------|------|
| **Amazon Quick** | AI-powered analytics platform (rebrand of QuickSight + AI assistant, Flows, Research, Index). No AWS account required. | [aws.amazon.com/quick](https://aws.amazon.com/quick/) |
| **Kiro** | Agentic IDE built by AWS — spec-driven development, Hooks, Steering, Powers, autonomous agent. Replaces Amazon Q Developer. | [kiro.dev](https://kiro.dev) |

---

## AWS Reference Architectures

| Resource | Link |
|----------|------|
| Multi-Agent Orchestration on AWS | [AWS Solutions Library](https://docs.aws.amazon.com/solutions/multi-agent-orchestration-on-aws/) |
| Agentic AI Operational Foundations | [AWS Solutions Library](https://docs.aws.amazon.com/solutions/agentic-ai-operational-foundations-on-aws/) |
| Intelligent Document Processing | [AWS Solutions Library](https://aws.amazon.com/solutions/guidance/intelligent-document-processing-on-aws/) |
| Supply Chain Data Hub | [AWS Solutions Library](https://docs.aws.amazon.com/solutions/deploying-a-supply-chain-data-hub-on-aws/) |
| Operationalizing Agentic AI | [Prescriptive Guidance](https://docs.aws.amazon.com/prescriptive-guidance/latest/strategy-operationalizing-agentic-ai/introduction.html) |
| Agentic AI Patterns & Workflows | [Prescriptive Guidance](https://docs.aws.amazon.com/prescriptive-guidance/latest/agentic-ai-patterns/introduction.html) |
| Building Serverless Agentic AI | [Prescriptive Guidance](https://docs.aws.amazon.com/prescriptive-guidance/latest/agentic-ai-serverless/introduction.html) |

---

## Architecture Diagrams (from repos)

| Diagram | Source |
|---------|--------|
| ![](https://raw.githubusercontent.com/aws-samples/sample-amazon-bedrock-agentcore-prototype-to-production/main/images/agentcore.png) | AgentCore Platform Overview |
| ![](https://raw.githubusercontent.com/awslabs/amazon-bedrock-agent-samples/main/examples/multi_agent_collaboration/support_agent/Support-Agent.png) | Customer Support Multi-Agent |
| ![](https://raw.githubusercontent.com/awslabs/agentcore-samples/main/02-use-cases/A2A-multi-agent-incident-response/images/architecture.png) | IT Ops — A2A Incident Response |
| ![](https://raw.githubusercontent.com/awslabs/agentcore-samples/main/02-use-cases/SRE-agent/docs/images/sre-agent-architecture.png) | IT Ops — SRE Agent |
| ![](https://raw.githubusercontent.com/aws-samples/sample-aws-idp-pipeline/main/docs/src/content/docs/assets/architecture.png) | Intelligent Document Processing |
| ![](https://raw.githubusercontent.com/aws-samples/sample-multi-agent-collaboration-with-strands/main/orchestration.png) | Multi-Agent Orchestration (Strands) |

---

> **AWS Agentic AI Incubator Program** — Wave 2, 2026
