# Liemo — Project Overview & Vision

*Live Store Link Aggregator Platform*

## 1.1 Problem Statement

The live commerce and online podcast-selling ecosystem has exploded across platforms like TikTok Shop, Facebook Live, Instagram, Shopee Live, and others. Sellers — particularly in high-growth markets like the Philippines and Kuwait — operate across multiple platforms simultaneously, making it nearly impossible for buyers to track their favorite stores in one place.

### Buyer Pain Points
- No centralized directory of live selling stores across platforms
- No way to know when a favorite store is currently live
- No category-based discovery (e.g., fashion, food, electronics)
- No trust signals like ratings, reviews, or verified badges
- Fragmented experience switching between TikTok, FB, IG, Shopee

### Store Owner Pain Points
- No analytics on which platform drives the most traffic
- No unified link management for promotions
- No subscriber or follower notification system across channels

## 1.2 The Solution — Liemo

Liemo is a multi-platform live store link aggregator that solves the discovery and management problem for both buyers and live sellers. Think of it as a 'Linktree for live sellers' with real-time status, ratings, category browsing, and a powerful analytics dashboard for store owners and super admins.

## 1.3 Target Markets

| Phase | Market | Language Support | Timeline |
|-------|--------|-----------------|----------|
| Phase 1 | Philippines | English / Filipino | Q3 2026 |
| Phase 2 | Kuwait | English / Arabic (RTL) | Q4 2026 |
| Phase 3 | Global Rollout | Multi-language | 2027 |

## 1.4 Business Model

| Revenue Stream | Target Actor | Description |
|---------------|-------------|-------------|
| Subscription (Basic/Pro/Enterprise) | Store Owners (Admin) | Monthly/annual plans unlocking analytics, featured listings, verified badge |
| Wallet Top-up & Credits | Store Owners | Credits for boosted visibility, push notifications to followers |
| In-app Advertising | Brands / Free Users | Banner and native ads shown to end users on free tier |
| Commission / Affiliate | Super Admin | Optional % cut on referred transactions (future phase) |

## 2. System Actors & Roles

| Actor | Platform | Key Capabilities |
|-------|----------|------------------|
| End User (Buyer) | Mobile App (Flutter) | Browse categories, search stores, view live status, rate stores, follow stores, see ads (free tier) |
| Store Admin (Seller) | Web App (React) | Manage store profile, add platform links, view analytics, manage subscription/wallet, respond to reviews |
| Super Admin | Web Dashboard (React) | Manage all users and admins, configure categories, view platform-wide analytics, manage ads, subscriptions, and system settings |
