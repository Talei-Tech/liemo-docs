# Core Data Model — PostgreSQL Entity Summary

| Entity / Table | Key Fields | Relationships |
|---------------|-----------|---------------|
| `users` | id, email, password_hash, role (USER/ADMIN/SUPERADMIN), is_verified, created_at | 1:1 → user_profiles, 1:1 → store_admins (if ADMIN) |
| `user_profiles` | user_id, display_name, avatar_url, preferred_language, country | belongs to users |
| `stores` | id, admin_id, name, slug, bio, logo_url, is_verified, is_live, avg_rating, status (ACTIVE/PENDING/SUSPENDED) | belongs to users (admin); M:M → categories |
| `store_links` | id, store_id, platform (TIKTOK/FB/IG/SHOPEE/etc.), url, label, click_count, display_order | belongs to stores |
| `categories` | id, name, slug, icon_url, parent_id (for sub-categories), is_active | M:M → stores |
| `store_categories` | store_id, category_id | junction: stores ↔ categories |
| `follows` | id, user_id, store_id, created_at | users follow stores |
| `ratings` | id, user_id, store_id, score (1-5), review_text, created_at | belongs to users, stores |
| `subscriptions` | id, store_id, plan_id, status, start_date, end_date, payment_ref | belongs to stores, plans |
| `subscription_plans` | id, name (FREE/PRO/ENTERPRISE), price_monthly, price_annual, features (JSONB) | 1:M → subscriptions |
| `wallet_accounts` | id, store_id, balance_credits, currency | belongs to stores |
| `wallet_transactions` | id, wallet_id, type (TOPUP/SPEND), amount, description, created_at | belongs to wallet_accounts |
| `advertisements` | id, title, image_url, target_url, start_date, end_date, impressions, clicks, status | managed by super admin |
| `notifications` | id, user_id, type, title, body, is_read, created_at, metadata (JSONB) | belongs to users |
| `analytics_events` | id, store_id, event_type (VIEW/LINK_CLICK/FOLLOW), platform, created_at | belongs to stores; aggregated for dashboard |
