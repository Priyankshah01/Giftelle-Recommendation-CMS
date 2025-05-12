# 🎁 Giftelle - Gift Recommendation CMS

*A content management system for admins to manage gifts, occasions, and user profiles, using smart recommendation logic.*

## ✨ Features
- **Gift Catalog**: CRUD operations for gifts (name, price, category, image).
- **Occasion Management**: Tag gifts for occasions (e.g., birthdays and anniversaries).
- **User Profiles**: Store preferences (interests, budget) for personalized recommendations.

## 🛠️ Tech Stack
- **Backend**: ASP.NET Core, Entity Framework (Code-First)
- **Frontend**: MVC with Razor Views
- **Database**: SQL Server / SQLite

## 📊 Database Schema (ERD)
```mermaid
erDiagram
    UserProfile ||--o{ Occasion : "1-M (User selects occasions)"
    Gift }|--|{ Occasion : "M-M (Gifts for occasions via GiftOccasion)"
