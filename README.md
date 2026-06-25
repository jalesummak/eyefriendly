# EyeFriendly — AI Vision Assistant for the Visually Impaired

> A multilingual multi-agent AI system that helps visually impaired 
> and low-vision users worldwide navigate documents, images, 
> and daily life — in any language.

## The Problem
2.2 billion people worldwide live with vision impairment. 
Existing tools are expensive, rigid, and rarely support non-English languages.
EyeFriendly bridges this gap with an accessible, multilingual AI agent.

## Solution
EyeFriendly uses Google's Agent Development Kit (ADK) to create 
a multi-agent system where specialized agents handle different needs:

- 📄 **Document Reader** — Simplifies forms, medicine labels, reports
- 🖼️ **Image Describer** — Describes photos uploaded by caregivers
- 🧭 **Navigation Agent** — Detects obstacles, gives directions
- 📅 **Daily Assistant** — Medicine reminders, schedule management

## Architecture
User (text/voice)

↓

eyefriendly_orchestrator (ADK)

├── document_reader   → Documents, forms, medicine labels

├── image_describer   → Photos uploaded by caregivers

├── navigation_agent  → Obstacles, directions

└── daily_assistant   → Reminders, schedule
## Key Concepts Demonstrated

| Concept | Implementation |
|---|---|
| Multi-agent system (ADK) | Orchestrator + 4 specialist agents |
| MCP Server | 4 tools: describe_image, read_document, detect_obstacle, get_directions |
| Agent Skill | Accessibility Communication Skill |
| Security | PII masking + dangerous request blocker + audit log |
| Evaluation | 5/5 automated tests passed |
| Multilingual | Auto-detects and responds in any language |

## Setup Instructions

1. Clone this repository
2. Install dependencies: `pip install google-adk mcp gtts`
3. Set your API key: `export GOOGLE_API_KEY=your_key_here`
4. Run the notebook: `eyefriendly.ipynb`

## Track

**Agents for Good** — Solving accessibility challenges for 2.2 billion visually impaired people worldwide.
