# 🏛️ The Gats Lab: 24/7 AI Workforce
> Building a fully autonomous agency run by AI agents on a hybrid home server infrastructure.

## 🚀 The Mission
지하실에서 동작하는 **24/7 자율 AI 에이전시** 구축을 목표로 합니다. 
단순한 자동화를 넘어, **Local LLM(Mac Studio)**의 프라이버시/연산 성능과 **Cloud LLM API**의 지능을 적절히 조합하여 비용 대비 최적의 성능(Cost-Effective Intelligence)을 뽑아내는 하이브리드 인프라를 지향합니다.

---

## 🏗️ Architecture: Hybrid AI Setup
Gats Lab은 서비스 계층과 연산 계층이 분리된 효율적인 구조를 가집니다.

```mermaid
graph LR
    classDef default fill:#1e293b,stroke:#94a3b8,stroke-width:1px,color:#fff
    classDef external fill:#000,stroke:#fff,stroke-width:2px,color:#fff
    classDef gateway fill:#b45309,stroke:#fcd34d,stroke-width:2px,color:#fff
    classDef app fill:#065f46,stroke:#34d399,stroke-width:2px,color:#fff
    classDef agent fill:#581c87,stroke:#c084fc,stroke-width:2px,color:#fff
    classDef ai_engine fill:#312e81,stroke:#818cf8,stroke-width:2px,color:#fff
    classDef infra fill:#334155,stroke:#64748b,stroke-width:1px,color:#e2e8f0

    User((User / Internet)):::external

    subgraph Home_Server ["🏠 Home Server (Main Host)"]
        direction TB
        subgraph Service_Layer ["Service & Logic Layer"]
            direction LR
            NPM[/"Nginx Proxy Manager"/]:::gateway
            subgraph Apps ["Web Services"]
                direction TB
                BlogApp["Gats Lab Logs"]:::app
                Portfolio["Portfolio"]:::app
            end
            GatsAI["🤖 Gats AI Agent<br/>(Orchestrator)"]:::agent
        end
        subgraph Infra_Layer ["Infrastructure (Docker)"]
            direction LR
            Portainer["Portainer"]:::infra
            Prometheus["Prometheus"]:::infra
            Grafana["Grafana"]:::infra
        end
    end

    subgraph Mac_Studio ["🍎 Mac Studio (AI Brain)"]
        direction TB
        LLM_Engine["Local LLM Engine<br/>(Qwen 2.5 / vLLM)"]:::ai_engine
        AI_Workflow["Hybrid Workflow<br/>(Local + Cloud API)"]:::ai_engine
    end

    User ==> NPM
    NPM --> BlogApp
    NPM --> Portfolio
    GatsAI <== "Inference API" ==> LLM_Engine
    linkStyle default stroke:#22d3ee,stroke-width:2px
