# 🧠 OpenClaw Super Memory (Hermes Mind Evolution)

[![ClawHub](https://img.shields.io/badge/ClawHub-super--memory-orange.svg)](https://clawhub.io/skills/super-memory)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![OpenClaw Version](https://img.shields.io/badge/OpenClaw-2026.6+-purple.svg)](https://github.com/openclaw/openclaw)

An advanced OpenClaw skill that unlocks a **closed-loop self-improvement cycle** and **durable memory persistence** for your AI agents, raising their reasoning, memory retention, and skill-synthesis capabilities to the level of **Nous Research's Hermes Agent**.

---

## 🌐 Tiếng Việt

### Giới thiệu
Mặc dù OpenClaw rất mạnh mẽ nhờ các kết nối đa dạng (Zalo, Telegram, Browser, Workboard), các Agent mặc định thường gặp tình trạng "mau quên" giữa các ngày do cơ chế dọn dẹp lịch sử hội thoại (compaction) hoặc thuật toán Dreaming tự động quá khắt khe. 

**super-memory** giải quyết triệt để vấn đề này bằng cách bổ sung một **vòng lặp học hỏi khép kín (closed-loop learning)**:
1. **Ghi nhớ chủ động**: Ép bot tự động cập nhật [MEMORY.md](file:///e:/williams/.openclaw/workspace-williams-2/MEMORY.md) thời gian thực ngay khi học được bài học mới, thay vì đợi cơ chế Dreaming quét qua ban đêm.
2. **Tự tổng hợp kỹ năng**: Hướng dẫn bot tự động đóng gói các đoạn script hữu ích thành các **Skill mới** lưu trong thư mục `skills/` và cập nhật vào `TOOLS.md`.
3. **Pha phản tư (Self-Reflection)**: Bot tự nhìn nhận hành vi ở cuối phiên làm việc để tối ưu hóa tri thức của mình.

### Cách cài đặt & Sử dụng
Chạy script cài đặt để tự động quét `openclaw.json` và cập nhật quy tắc này vào toàn bộ các Agent đang hoạt động:
```bash
node install.js
```

Để khôi phục trạng thái ban đầu của các file `AGENTS.md`:
```bash
node install.js --restore
```

---

## 🇺🇸 English

### Overview
While OpenClaw excels at integrations (WhatsApp, Zalo, Telegram, Browser, Workboard), default agents often suffer from "amnesia" across sessions due to aggressive context compaction or overly strict automatic Dreaming threshold filters.

**super-memory** solves this by injecting a **closed-loop self-improvement loop** directly into your agent's system prompt:
1. **Durable Memory Synthesis**: Forces the agent to proactively write critical context, preferences, and bug fixes directly to `MEMORY.md` in real-time, bypassing passive dreaming filters.
2. **Autonomous Skill Creation**: Prompts the agent to crystallize successful complex workflows into reusable JS script files under the `skills/` folder and index them in `TOOLS.md`.
3. **Self-Reflection Loop**: Directs the agent to perform a final review step at the end of major sessions to prune, refine, and upgrade its own knowledge base.

### Installation & Usage
Run the install script to automatically scan `openclaw.json`, locate all active agent workspaces, and apply the memory-evolution prompts to their `AGENTS.md`:
```bash
node install.js
```

To roll back all modified files to their original state:
```bash
node install.js --restore
```

## 📂 Directory Structure
```text
openclaw-skill-super-memory/
├── .agent/
│   └── workflows/
│       └── update.md       # Release workflow instructions
├── scripts/
│   └── publish.js          # ClawHub publisher script
├── install.js              # Multi-agent workspace patcher
├── SKILL.md                # System prompt instructions
├── README.md               # User manual (SEO Optimized)
└── package.json            # NPM & ClawHub metadata
```

## 📄 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
