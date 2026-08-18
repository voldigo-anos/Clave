![Clave App Banner](https://res.cloudinary.com/dwcwp9ebv/image/upload/clave-repo_wsrmkq.jpg)

# ![Batman](https://cdn-icons-png.flaticon.com/32/15468/15468240.png) Clave App - Votre Sanctuaire IA Personnel

![Node.js](https://img.shields.io/badge/Node.js-v18%2B-brightgreen?style=flat-square&logo=node.js)
![Express](https://img.shields.io/badge/Express-v4.18-blue?style=flat-square&logo=express)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-CSS-38bdf8?style=flat-square&logo=tailwind-css)
![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)
![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-orange?style=flat-square)
![Maintained](https://img.shields.io/badge/Maintained-Yes-success?style=flat-square)

## ![](https://cdn-icons-png.flaticon.com/32/2339/2339864.png) Bienvenue sur Clave App

Bienvenue sur **Clave App** - une interface IA sophistiquée et axée sur la confidentialité, conçue pour les développeurs et les passionnés qui souhaitent un environnement propre et puissant pour interagir avec divers modèles d'IA sans le superflu.

Conçu dans un souci d'extensibilité et de personnalisation, Clave App sert de "Clave" personnelle où vous pouvez réfléchir, créer et explorer des idées avec l'assistance de l'IA. Que vous cherchiez à déployer votre propre interface de chat privée, à créer un outil IA personnalisé, ou à apprendre à intégrer plusieurs modèles d'IA dans une application Node.js, Clave App constitue la base idéale.

## ![](https://cdn-icons-png.flaticon.com/32/8589/8589419.png) Fonctionnalités clés

*   **Support multi-modèles :** Intégration transparente avec GPT-4o, GPT-3.5 et d'autres modèles d'IA de premier plan
*   **Génération d'images avancée :** Créez des visuels impressionnants avec les modèles DeepImg et Flux
*   **UI/UX élégante :** Interface en mode sombre, sans distraction, construite avec EJS et Tailwind CSS
*   **API complète :** API RESTful entièrement documentée avec validation robuste, gestion des erreurs et fonctionnalités de sécurité
*   **Centré sur le développeur :** Conçu pour être facilement forké, personnalisé et déployé
*   **Architecture extensible :** Base de code modulaire qui simplifie l'ajout de nouvelles fonctionnalités et de nouveaux modèles

## ![](https://cdn-icons-png.flaticon.com/32/7364/7364295.png) Stack technique

*   **Environnement d'exécution :** [Node.js](https://nodejs.org/) (v18 ou supérieur)
*   **Framework web :** [Express.js](https://expressjs.com/)
*   **Moteur de templates :** [EJS](https://ejs.co/)
*   **Framework de style :** [Tailwind CSS](https://tailwindcss.com/)
*   **Bibliothèque d'icônes :** [Lucide Icons](https://lucide.dev/)
*   **Coloration syntaxique :** [Highlight.js](https://highlightjs.org/)

## ![](https://cdn-icons-png.flaticon.com/32/675/675579.png) Guide de démarrage rapide

### Prérequis

*   Node.js (v18 ou supérieur recommandé)
*   Gestionnaire de paquets npm ou yarn
*   Clés API pour les services d'IA souhaités

### Installation et configuration

1.  **Forker et cloner le dépôt**
    Commencez par forker ce dépôt sur votre compte GitHub, puis clonez-le en local :
    ```bash
    git clone https://github.com/voldigo-anos/Clave.git
    cd Clave
    ```

2.  **Installer les dépendances**
    Installez tous les paquets requis avec npm :
    ```bash
    npm install
    ```

3.  **Lancer l'application**
    Démarrez le serveur de développement :
    ```bash
    npm start
    ```
    Accédez à l'application sur `http://localhost:3000` et commencez à explorer votre sanctuaire IA.

## ![](https://cdn-icons-png.flaticon.com/32/3815/3815573.png) Options de personnalisation

Clave App est conçu pour la flexibilité et la personnalisation :

*   **Marque et identité :** Modifiez `config/webConfig.json` pour personnaliser le nom du site, la description, les icônes et les couleurs du thème
*   **Intégration de modèles IA :** Gérez les configurations des modèles dans `config/models.js` pour ajouter ou supprimer des services d'IA
*   **Style UI/UX :** Exploitez Tailwind CSS pour des ajustements de style complets dans `public/css` avec les templates de vues dans `views/`
*   **Extensions API :** Étendez les fonctionnalités en ajoutant de nouveaux contrôleurs dans `controllers/` et des routes dans `routes/`

## ![](https://cdn-icons-png.flaticon.com/32/8297/8297437.png) Documentation de l'API

Une documentation complète de l'API est disponible dans l'application. Une fois votre serveur lancé, rendez-vous sur `/docs` (par exemple, `http://localhost:3000/docs`) pour une référence API interactive.

### Points de terminaison principaux

*   `POST /api/chat` - Complétions de chat avancées avec historique de conversation
*   `POST /api/image` - Génération d'images de haute qualité avec options de style
*   `POST /api/reset` - Effacement sécurisé de l'historique de conversation
*   `GET /api/status` - Surveillance de l'état et de la santé du système

## ![](https://cdn-icons-png.flaticon.com/32/17379/17379046.png) Exemples de code

Voici comment interagir avec l'API en utilisant des langages courants :

### JavaScript (Fetch)

```javascript
const response = await fetch('http://localhost:3000/api/chat', {
  method: 'POST',
  headers: {
    'Content-Type': 'application/json',
    'x-session-id': 'my-session-123'
  },
  body: JSON.stringify({
    message: 'Hello, how are you?',
    model: 'gpt-3.5'
  })
});

const data = await response.json();
console.log(data.text);
```

### Python (Requests)

```python
import requests

url = "http://localhost:3000/api/chat"
headers = {
    "Content-Type": "application/json",
    "x-session-id": "my-session-123"
}
data = {
    "message": "Tell me a joke",
    "model": "gpt-4o"
}

response = requests.post(url, json=data, headers=headers)
print(response.json()["text"])
```

## ![](https://cdn-icons-png.flaticon.com/32/17942/17942509.png) Feuille de route de développement

Améliorations actuelles et prévues pour Clave App :

- [x] **Phase 1 :** Implémentation de l'interface de chat de base
- [x] **Phase 2 :** Fonctionnalités de génération d'images
- [x] **Phase 3 :** Documentation complète de l'API
- [x] **Phase 4 :** Gestion globale robuste des erreurs
- [x] **Phase 5 :** Validation des entrées et en-têtes de sécurité
- [ ] **Phase 6 :** Streaming des réponses
- [ ] **Phase 7 :** Améliorations du rendu Markdown
- [ ] **Phase 8 :** Bascule mode sombre/clair

## ![](https://cdn-icons-png.flaticon.com/32/10703/10703030.png) Fonctionnalités de sécurité

Nous prenons la sécurité très au sérieux. Clave App intègre une protection dès sa conception :

*   **Validation des entrées :** Middleware de validation complet pour tous les points de terminaison de l'API.
*   **Protection XSS :** Assainissement automatique des entrées utilisateur.
*   **Journalisation sécurisée :** Les données sensibles (clés API, mots de passe) sont automatiquement masquées dans les journaux.
*   **Gestion des erreurs :** Réponses d'erreur sécurisées pour la production qui ne divulguent pas les traces de pile.
*   **En-têtes :** En-têtes de sécurité configurés selon les meilleures pratiques.

## ![](https://cdn-icons-png.flaticon.com/32/3735/3735057.png) Structure du projet

```
Clave-App/
├── config/             # Fichiers de configuration (modèles, paramètres web)
├── controllers/        # Gestionnaires de requêtes (chat, image, utilitaire)
├── lib/                # Implémentations des modèles d'IA
├── middleware/         # Middleware Express (logger, erreur, validateur)
├── public/             # Ressources statiques (css, js, images)
├── routes/             # Routes API et de vues
├── views/              # Templates EJS
└── server.js           # Point d'entrée de l'application
```

## ![](https://cdn-icons-png.flaticon.com/32/8765/8765344.png) Communauté et contributions

Nous accueillons les contributions de la communauté des développeurs. Pour contribuer :

1.  **Forkez** le dépôt
2.  Créez une branche de fonctionnalité (`git checkout -b feature/amazing-enhancement`)
3.  Validez vos modifications (`git commit -m 'Add amazing enhancement'`)
4.  Poussez vers votre branche (`git push origin feature/amazing-enhancement`)
5.  Ouvrez une **Pull Request** avec une description détaillée

Veuillez consulter nos [directives de contribution](CONTRIBUTING.md) avant de soumettre des pull requests.

Consultez [CHANGELOG.md](CHANGELOG.md) pour plus de détails sur les versions et les modifications.

## ![](https://cdn-icons-png.flaticon.com/32/1828/1828884.png) Soutenir le projet

Si Clave App a bénéficié à votre flux de travail ou inspiré vos projets, veuillez envisager de montrer votre soutien :

*   ⭐ Mettez une étoile à ce dépôt sur GitHub
*   🐦 Suivez le mainteneur sur Twitter [@1dev_hridoy](https://twitter.com/1dev_hridoy)
*   💬 Partagez votre expérience avec d'autres membres de la communauté des développeurs

## ![](https://cdn-icons-png.flaticon.com/32/3135/3135748.png) Licence et mentions légales

Ce projet est distribué sous la [licence MIT](LICENSE), permissive, autorisant l'usage commercial, la modification, la distribution et l'usage de brevets. Voir le fichier [LICENSE](LICENSE) pour les termes complets.

---

<div align="center">
  <sub>Créé avec ❤️ par <a href="https://github.com/voldigo-anos">Voldy</a> 
  
