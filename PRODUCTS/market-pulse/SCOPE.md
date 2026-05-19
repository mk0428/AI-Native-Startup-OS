# Market Pulse — SCOPE

## 1. The Problem
Indie developers and small teams need weekly competitive intelligence (who's rising, what's trending, what's new) but can't afford Sensor Tower ($100-500/mo) or similar tools. They currently do nothing or manually browse App Store.

## 2. The Solution
A bot that delivers weekly market briefs to your chat (Telegram/Feishu/Slack). No dashboard to learn. No login to remember. Data comes to you.

**Core interaction:**
```
User subscribes → Bot delivers weekly report → User reads in 30 seconds → Gets signal
```

## 3. Scope
**DO:** Weekly App Store Top 50 reports for 3 categories. Payment via Gumroad. Landing page on Vercel.
**DON'T:** Build a dashboard. Support Google Play (yet). Add keyword/download data (yet).

## 4. Unit Economics
| Item | Cost |
|------|------|
| API/RSS | $0 |
| Server | Already paid (Aliyun) |
| Gumroad fee | 8.5% + $0.30/transaction |
| **Cost per user/month** | **~$0** |

| Pricing | Users to $100/mo |
|---------|-----------------|
| $19/mo | 6 |
| $190/yr | 6 (annual) |

## 5. Success Criteria
**Week 1:** Landing page live + Gumroad active
**Month 1:** 1 paying subscriber or Product Hunt 50+ upvotes → continue
**Kill condition:** 0 subscribers after 30 days → archive

## 6. Counterarguments
1. Indie devs don't pay for tools → Price at $19 and find out
2. Data is too thin → We can add more categories/sources later
3. Already free alternatives exist (manual browsing) → Yes, but people don't do it consistently
