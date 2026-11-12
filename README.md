# LAB 1 — Conception et test d’une API REST

TP sur DummyJSON avec Postman, réalisé par Mohammed Noureddine.

## Lancer le TP

1. Importer `LAB1.postman_collection.json` et `Demo_API_Env.postman_environment.json` dans Postman.
2. Sélectionner **Demo API Env**, ouvrir **LAB1 - Gestion Produits REST** et cliquer sur **Run collection**.
3. Consulter les assertions dans les résultats du Runner et les observations dans `Rapport_LAB1.pdf`.

Exécution en ligne de commande avec Newman

```sh
npx newman run LAB1.postman_collection.json -e Demo_API_Env.postman_environment.json
```

La campagne a exécuté 11 requêtes et validé 23 assertions sur 24. Le seuil de 500 ms a échoué avec 3 866 ms sur la requête smartphones. Les écritures de DummyJSON sont simulées.
