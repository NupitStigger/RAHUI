# RAHUI Project
Проект на стеке **Go (Backend)** и **Next.js (Frontend)**.

## 📊 Схема базы данных (ER-диаграмма)

```mermaid
erDiagram
    USER ||--o{ TASK : creates
    USER {
        int id PK
        string username
        string email
        string password_hash
        datetime created_at
    }
    TASK {
        int id PK
        int user_id FK
        string title
        string status
        datetime created_at
    }
