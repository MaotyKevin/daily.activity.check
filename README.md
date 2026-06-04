# 🟩 Daily Auto Commit Bot

A GitHub Actions bot that automatically commits to this repository every day to maintain a consistent contribution streak on my GitHub profile.

---

## How It Works

A scheduled GitHub Actions workflow runs every day at **01:40 am UTC+3**. It appends a timestamped line to `activity_log.txt`, then commits and pushes it — generating a green square on the contribution graph automatically.

No manual action needed. It runs forever on its own.

---

## Workflow Schedule

| Trigger | Time |
|---|---|
| Automatic | Every day at 12:00 UTC |
| Manual | Available via the Actions tab (workflow_dispatch) |

---

## Repository Structure

```
.
├── .github/
│   └── workflows/
│       └── daily-commit.yml   # The automation workflow
├── activity_log.txt           # Auto-generated daily log
└── README.md                  # This file
```

---

## GitHub Actions Usage

This workflow uses approximately **~62 minutes/month** out of the **2,000 free minutes** provided by GitHub — roughly 3% of the free quota.

For public repositories, Actions minutes are **unlimited**.

---

## Setup (already done)

1. ✅ Created the repository
2. ✅ Enabled **Read and write permissions** under Settings → Actions → General
3. ✅ Added `.github/workflows/daily-commit.yml`
4. ✅ Tested manually via the Actions tab
