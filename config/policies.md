# OpenClaw Operational Policies

- **Model Usage:** Prioritize `deepseek/chat` for speed on simple Q&A. Fallback to `deepseek/reasoner` or `openrouter/auto` for complex tasks. All models must be free-tier.
- **Secrets Management:** Store tokens in GitHub Secrets or local credentials (`~/.openclaw/credentials/`); NEVER commit tokens to the repo.
- **Security:** Sandbox mode is `all`; web tools are denied (`tools.deny = ["group:web"]`).
- **GitHub Integration:** Webhooks and Actions automate builds and deployments triggered by pushes to the default branch.
