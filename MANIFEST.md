# VULKN Agent Skill Bundle 🚀

This repository contains the standard "Battle-Ready" skills for VULKN cloud agents.

## 📦 Included Skills
1. **Google Official:** Full SDK access to Gmail, Calendar, Drive, and Sheets.
2. **Nano Banana Pro:** High-speed image generation and editing via Gemini.
3. **Summarize:** Multimodal video/URL analysis and transcription.
4. **Veo Gen:** Official Google Veo 3.1 video generation.
5. **Firecrawl:** Advanced search and markdown extraction.
6. **Twilio Voice & SMS:** Telephony interface for calls and reminders.
7. **ManyChat Bridge:** Bridge to Facebook/Instagram DM automation.

## 🛠️ Installation
Run this one-liner in your `~/.openclaw/workspace/skills` directory:
```bash
git clone https://github.com/sybil-bjs/vulkn-agent-bundle.git .bundle && cp -r .bundle/* . && rm -rf .bundle
```

## 🔑 Required Keys (Add to your .env)
### Core AI
- `GEMINI_API_KEY`: For Images, Video, and Veo.
- `FIRECRAWL_API_KEY`: For advanced research.

### Telephony (Twilio)
- `TWILIO_ACCOUNT_SID`: `[See VULKN Secure Vault]`
- `TWILIO_AUTH_TOKEN`: `[See VULKN Secure Vault]`
- `TWILIO_PHONE_NUMBER`: `[See VULKN Secure Vault]`

### Social & Automation (ManyChat)
- `MANYCHAT_API_KEY`: Format `123456:abcdef...`
- `MANYCHAT_BASE_URL`: Usually `https://api.manychat.com/fb/` for v1.

## 🚀 Usage Tips
- **Twilio:** Use the `twilio` CLI or the `twilio-voice` skill for phone calls.
- **ManyChat:** Use the `/fb/page/getInfo` endpoint to verify connectivity.
- **Google:** Always specify the `subject` email if using Domain-Wide Delegation.
