## Prérequis

Créer le secret Postgres avant de déployer :

```bash
kubectl create secret generic db-credentials -n voting-app \
  --from-literal=POSTGRES_USER=postgres \
  --from-literal=POSTGRES_PASSWORD=<mot-de-passe>
```