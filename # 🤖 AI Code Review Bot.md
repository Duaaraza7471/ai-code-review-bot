# 🤖 AI Code Review Bot
Automated AI-powered code review for every GitHub pull request — feedback in seconds, not days.

## 🎯 The Problem
Manual code reviews are slow (200–400 lines/hour), inconsistent, and repetitive.
Bugs and bad practices slip through. Junior devs wait days for feedback.

## 💡 The Solution
A bot that instantly reviews every PR:
- 🔍 Detects bugs & bad practices (bare `except:`, `== None`, hardcoded secrets, TODOs)
- 💡 Suggests fixes with explanations — powered by AI
- ⚡ Reviews in &lt; 10 seconds, 24/7
- 🔗 Native GitHub integration via webhooks

## ⚙️ How It Works
PR opened → GitHub webhook → Bot analyzes the diff (AST + static checks + LLM) →
Inline review comments with fix suggestions posted back on the PR

## 🚀 Quick Start (Prototype)
```bash
git clone https://github.com/duaaraza7471/ai-code-review-bot.git
cd ai-code-review-bot
python review.py sample_bad_code.py