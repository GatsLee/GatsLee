# GatsLee — AI Engineer & Builder

Solo builder shipping AI products across iOS, macOS, and home infrastructure.
iOS · macOS · 홈서버를 넘나들며 AI 제품을 직접 만들고 출시하는 1인 빌더.

📝 [blog.gatslee.com](https://blog.gatslee.com) — 내가 만드는 모든 것의 기록

---

## 🚀 Featured Projects

### [Calyx](https://blog.gatslee.com/products/calyx) — Well-being Calendar Agent
> One AI agent looking after your entire calendar — sleep, meals, movement, rest, focus.
> 수면 · 식사 · 운동 · 휴식 · 집중 다섯 영역을 동시에 보는 AI 캘린더 에이전트.

- **Stack**: Swift · SwiftUI · iOS 17+ · watchOS · FastAPI · SQLite (GRDB) · HealthKit · EventKit · StoreKit 2
- **Status**: TestFlight beta (v0.2)

### [Alfred](https://blog.gatslee.com/about) — Personal AI Archive Agent
> A local-first AI butler that remembers everything — voice, photos, chats, files.
> 음성 · 카메라 · 키보드 · 파일 네 채널로 모든 것을 기억하는 로컬 퍼스트 AI 집사.

- **Stack**: Python · Ollama (Gemma) · LightRAG · SQLite / PostgreSQL · Textual TUI · MCP
- **Status**: Active development (386 tests passing)

### [The Gats Lab](https://blog.gatslee.com/) — My Living Portfolio
> blog.gatslee.com itself is a product I designed and ship end-to-end.
> 블로그 자체가 살아있는 포트폴리오 — 설계·구현·운영 모두 혼자.

- **직접 설계한 RAG 아키텍처** — FAQ 라우터 → 벡터 검색 → LLM 생성, 3티어 파이프라인을 처음부터 구현
- **GPU 인프라 직접 운영** — Ollama + NVIDIA GPU 컨테이너를 홈서버에 구성, 동시성 제어와 레이트 리밋까지
- **풀스택 단독 구현** — 프론트엔드(블록 에디터, 애니메이션, i18n) · 백엔드(인증, API, 마이그레이션) · 인프라(Docker, 배포 자동화)
- **Living product** — 방문자가 챗봇에 질문하고, 커밋 히스토리와 빌드 타임라인이 실시간 반영

---

## 🛠️ Tech Stack

- **Languages** — Swift · Python · TypeScript
- **AI / ML** — LLM orchestration · RAG (LightRAG) · Ollama · vLLM · MCP
- **iOS / macOS** — SwiftUI · `@Observable` (iOS 17+) · HealthKit · EventKit · StoreKit 2 · watchOS
- **Backend** — FastAPI · SQLite (GRDB) · PostgreSQL · Google Cloud Run
- **Infra** — Docker · Nginx Proxy Manager · NVIDIA GPU · Portainer · Prometheus · Grafana

---

## ⚒️ Now Building

- **Calyx v0.2** — Diet / Workout / Relax 모듈 + Apple Watch 앱 + StoreKit 2 Pro
- **Alfred** — 민감도 라우터 + ReAct 로컬 에이전트 확장
- **The Gats Lab** — RAG 파이프라인 고도화 + 포트폴리오 UX

---

## 📫 Contact

- 📝 Blog — [blog.gatslee.com](https://blog.gatslee.com)
- ✉️ Email — [naanthonylee@gmail.com](mailto:naanthonylee@gmail.com)
- 💼 LinkedIn — [joon-yeol-lee](https://www.linkedin.com/in/joon-yeol-lee-567421281/)
