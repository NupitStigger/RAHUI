# RAHUI Project
# 🚀 Project Management & Infrastructure Plan 2025

## 1. Жобаны басқару (Linear & Scrum)
* **Әдістеме:** Scrum (2 апталық спринттер).
* **Құрал:** [Linear Workspace](https://linear.app/rahman) — тапсырмаларды қадағалау және жоспарлау.
* **Процесс:** Бэклогты басқару, күнделікті синхрондау және спринт ретроспективасы.

## 2. Технологиялық стек
* **Frontend:** Next.js (React framework).
* **Backend:** Go (API қызметтері).
* **Деректер базасы:** PostgreSQL (dbdiagram.io арқылы жобаланған).
* **Инфрақұрылым:** Docker (контейнерлеу) және Terraform (IaC).

## 3. Архитектуралық схема
```mermaid
graph TD
    User((Пайдаланушы)) --> FE[Next.js Frontend]
    FE --> BE[Go API Service]
    BE --> DB[(PostgreSQL Database)]
    Linear[Linear: Task Management] -.-> BE
    Actions[GitHub Actions: CI/CD] --> Docker[Docker Image]
    Docker --> Cloud[Terraform: Infrastructure]
