# snowddl-practice

Projet de pratique SnowDDL : gestion déclarative d'objets Snowflake (warehouses, databases, schemas, rôles, users) par brique.

## Setup

```bash
python3 -m venv venv
source venv/bin/activate
pip install snowddl
```

Copier `.env.example` en `.env` et remplir les identifiants Snowflake (jamais commiter `.env`).

## Usage

```bash
set -a && source .env && set +a
snowddl -c config plan
snowddl -c config apply
```
