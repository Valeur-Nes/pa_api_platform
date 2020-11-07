####Projet-annuel Back END

### JWT auth

Génération d'un mdp via commande : 
```
docker-compose exec php bin/console security:encode-password
```
Connexion pour get un token JWT
```
curl -kX POST -H "Content-Type: application/json" https://localhost:8443/authentication_token -d '{"email":"amorin@suchweb.fr","password":"test"}'
```
Utilisation du token get précédement
```
Bearer YOUR_TOKEN_HERE
```
