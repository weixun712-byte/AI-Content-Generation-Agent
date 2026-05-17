# ✨ AI Content Generation Agent

企业级 AI 内容生成与发布平台

## 项目简介

AI Content Generation Agent 是一个基于 Multi-Agent 架构的企业级内容创作平台，能够实现从创意生成、文案撰写、编辑优化到自动发布的完整闭环。

## 核心能力

* **Idea Agent**：根据需求生成创意与内容大纲
* **Writer Agent**：自动撰写营销文案、博客文章和社交媒体内容
* **Editor Agent**：优化文本风格、语法和逻辑
* **Publisher Agent**：自动发布内容并生成发布报告
* **RAG 企业知识库支持**：定制化内容生成
* **多模型接入**：OpenAI / Claude / Gemini
* **Workflow 编排**：任务流自动化和调度
* **Token 消耗统计**：实时监控AI调用成本

## 技术栈

* Backend: FastAPI, LangChain, PostgreSQL
* Frontend: Next.js, React, TailwindCSS
* Deployment: Docker, Docker Compose

## 项目结构

```bash
AI-Content-Agent/
├── backend/
│   ├── app/
│   │   ├── main.py
│   │   ├── routes/
│   │   └── services/
│   └── requirements.txt
├── frontend/
│   ├── pages/
│   └── package.json
├── docker-compose.yml
└── README.md
```

## 快速启动

### Backend

```bash
cd backend
pip install -r requirements.txt
uvicorn app.main:app --reload
```

访问: `http://localhost:8000`

### Frontend

```bash
cd frontend
npm install
npm run dev
```

访问: `http://localhost:3000`

### Docker 部署

```bash
docker-compose up --build
```

## API 示例

### 执行内容生成任务

**POST** `/api/agent/run`

Request Body:

```json
{
  "task": "生成一篇关于新品发布的营销文案"
}
```

Response:

```json
{
  "idea": "新品发布创意方案",
  "content": "完整营销文案",
  "editor_notes": "文本优化建议",
  "publish_status": "已发布"
}
```

## MVP 落地方向

* 企业营销文案自动生成
* 社交媒体自动化运营
* 博客与文章内容自动生成
* 自动排版和发布监控

## 安全与权限

* JWT 鉴权
* RBAC 权限控制
* API Key 管理
* 发布审计日志

## License

MIT

## 作者

AI Content Generation Agent MVP Team
