# RAHUI Project
# 🚀 Project Management & Infrastructure Plan 2025

## 1. Жобаны басқару (Management)
* **Әдістеме:** Scrum (2 апталық спринттер).
* **Құрал:** [Linear Board](https://linear.app/rahman) — тапсырмалар мен спринттерді басқару.
* **Рөлдер:** PM (үйлестіру), Analyst (API спецификациясы), Backend/Frontend (әзірлеу), DevOps (инфрақұрылым).

## 2. Технологиялық стек
* **Frontend:** Next.js.
* **Backend:** Go (Golang).
* **База:** PostgreSQL (dbdiagram.io арқылы жобаланған).
* **Инфрақұрылым:** Docker, Terraform.

## 3. Архитектуралық схема
```mermaid
graph TD
    User((Пайдаланушы)) --> FE[Next.js Frontend]
    FE --> BE[Go API Gateway]
    BE --> DB[(PostgreSQL)]
    Linear[Linear: Task Tracking] -.-> BE
    Actions[GitHub Actions: CI/CD] --> Docker[Docker Image]
    Docker --> Cloud[Terraform: Cloud Infra]
