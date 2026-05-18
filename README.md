# 📦 Taskfile Laravel Docker Lab

Projet d’apprentissage de **Taskfile.dev** dans un environnement **Docker + Laravel**, avec une comparaison directe avec les **Makefiles traditionnels**.

L’objectif est de moderniser l’automatisation des commandes de développement et d’améliorer la **Developer Experience (DX)**.

---

# 🎯 Objectif du projet

Ce projet sert à :

- Apprendre et expérimenter **Taskfile.dev**
- Remplacer progressivement les usages de **Makefile**
- Centraliser les commandes Docker + Laravel
- Standardiser les workflows de développement
- Améliorer la lisibilité et la maintenabilité des scripts

---

# ⚙️ Stack technique

- Laravel
- Docker / Docker Compose
- Taskfile.dev
- PostgreSQL (ou MySQL selon config)
- Nginx
- PHP 8.4+
- Composer

---

# 📊 Makefile vs Taskfile

## ❌ Makefile (approche traditionnelle)

Makefile est puissant mais présente plusieurs limites dans un projet moderne.

### Exemple Makefile

```makefile
up:
	docker compose up -d

migrate:
	docker compose exec app php artisan migrate

test:
	docker compose exec app php artisan test