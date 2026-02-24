# VULKN Agent Skill Bundle 🚀

This repository contains the standard "Battle-Ready" skills for VULKN cloud agents.

## 📦 Included Skills
1. **Google Official:** Full SDK access to Gmail, Calendar, Drive, and Sheets.
2. **Nano Banana Pro:** High-speed image generation and editing via Gemini.
3. **Summarize:** Multimodal video/URL analysis and transcription.
4. **Veo Gen:** Official Google Veo 3.1 video generation.
5. **Firecrawl:** Advanced search and markdown extraction.

## 🛠️ Installation
Run this one-liner in your `~/.openclaw/workspace/skills` directory:
```bash
git clone https://github.com/sybil-bjs/vulkn-agent-bundle.git .bundle && cp -r .bundle/* . && rm -rf .bundle
```

## 🔑 Required Keys (Add to your .env)
- `GEMINI_API_KEY`: For Images, Video, and Veo.
- `FIRECRAWL_API_KEY`: For advanced research.
- `TWILIO_ACCOUNT_SID` / `TWILIO_AUTH_TOKEN`: For voice and SMS.
- `MANYCHAT_API_KEY`: For DM automation.
