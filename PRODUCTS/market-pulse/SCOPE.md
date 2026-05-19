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
**DO:** Weekly App Store Top 50 reports for 3 categories. Payment via Stripe. Landing page on Vercel.
**DON'T:** Build a dashboard. Support Google Play (yet). Add keyword/download data (yet).

## 4. Unit Economics
| Item | Cost |
|------|------|
| API/RSS | $0 |
| Server | Already paid (Aliyun) |
| Stripe fee | 2.9% + $0.30/transaction |
| **Cost per user/month** | **~$0** |

| Pricing | Users to $100/mo |
|---------|-----------------|
| $9/mo | 12 |
| $89/yr | 14 (annual) |

## 5. Success Criteria
**Week 1:** Landing page live + Stripe active ✅ (Deployed 2026-05-19)
**Month 1:** 1 paying subscriber or Product Hunt 50+ upvotes → continue
**Kill condition:** 0 subscribers after 30 days → archive

## 6. Counterarguments
1. Indie devs don't pay for tools → Priced at $9/mo (impulse buy range)
2. Data is too thin → We can add more categories/sources later
3. Already free alternatives exist (manual browsing) → People don't do it consistently

## Status: 🟢 Live — MVP Stage (accepting payments)
- Landing: https://market-pulse-landing.vercel.app
- Stripe: Monthly $9 (price_1TYkHpBlpAKmQ4kNneTNWpu2), Yearly $89 (price_1TYkHqBlpAKmQ4kNHFkZFWdU)
- Data collection: Daily UTC 2:00 on Aliyun
- Delivery: Weekly Monday 10AM via Hermes cron → Feishu
