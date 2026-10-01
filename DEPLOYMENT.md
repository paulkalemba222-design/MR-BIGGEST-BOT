# 🦁 So Biggest — Déploiement

## 1. Vercel
Importe le dépôt dans Vercel pour mettre en ligne la partie API/web.

La route `/api/health` permet de vérifier que l'API répond.

## 2. Worker WhatsApp
Le bot WhatsApp Baileys doit être lancé sur un service Node.js persistant.

Dans `worker/` :

```bash
npm install
npm start
```

Variables :

```env
PREFIXE=.
DOSSIER_AUTH=auth_baileys
NUMBER=243849360396
BOT_NUMBER=243849360396
USE_PAIRING_CODE=true
RECONNECT_DELAY=5000
```

Le premier démarrage affiche le code de liaison dans les logs.

## 3. Session
Le dossier `auth_baileys` doit rester persistant. Ne le publie pas sur GitHub.
