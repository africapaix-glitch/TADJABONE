[![license](https://img.shields.io/badge/license-MIT-green.svg)](./LICENSE) [![release](https://img.shields.io/github/v/release/africapaix-glitch/TADJABONE)](https://github.com/africapaix-glitch/TADJABONE/releases) [![build](https://img.shields.io/github/actions/workflow/status/africapaix-glitch/TADJABONE/ci.yml?branch=main)](https://github.com/africapaix-glitch/TADJABONE/actions)

# TADJABONE

TADJABONE est une application légère de gestion d'un centre d'accompagnement scolaire (inscriptions, fréquentation, bibliothèque, prêts, partenaires et communications). Elle est conçue comme une SPA React avec une persistance simple en localStorage pour un déploiement et un démarrage rapides.

Principales fonctionnalités
- Inscription publique des élèves (formulaire public)
- Interface administrateur (tableau de bord, gestion des élèves, fréquentation, bibliothèque, prêts)
- Gestion des partenaires et communications (envoi de messages / rappels)
- Génération de carte d'identité élève (ID Card) et QR Code d'accès mobile
- Assistant IA local pour analyses et suggestions (fonctionnalité interne)

Technologies
- React
- Tailwind CSS (styles utilitaires)
- lucide-react (icônes)
- localStorage pour la persistance locale des données

Installation locale
1. Clonez le dépôt:
   git clone https://github.com/africapaix-glitch/TADJABONE.git
2. Entrez dans le dossier du projet:
   cd TADJABONE
3. Installez les dépendances:
   npm install
   # ou
   yarn install
4. Démarrez l'application en mode développement:
   npm run dev
   # ou selon le script présent dans package.json

Remarques d'utilisation
- Données: L'application utilise localStorage (tadjabone_students, tadjabone_books, etc.). Les données sont persistées dans le navigateur et ne sont pas synchronisées côté serveur.
- Modes: Il y a deux modes principaux — public (inscription, consultation de carte) et administrateur (accès complet après connexion admin).
- QR Code: L'interface admin permet de générer un QR Code pointant vers l'URL courante pour un accès mobile simple.

Structure du projet (exemples)
- src/
  - components/  -> Composants React réutilisables (Dashboard, StudentList, StudentForm, LibraryManager, etc.)
  - types.ts     -> Définitions TypeScript des types utilisés (Student, AttendanceRecord, Book, Loan, Partner, Communication)
  - App.tsx      -> Point d'entrée principal de l'interface (logique d'état, routes internes)

Comment contribuer
- Ouvrez une issue pour proposer un changement ou signaler un bug.
- Créez une branche feature/bugfix à partir de main et ouvrez une pull request détaillant vos changements.

Licence
- Ajoutez la licence souhaitée (ex. MIT) ou contactez le mainteneur du dépôt pour plus d'information.

---

Fichiers ajoutés/ mis à jour : .github/CODEOWNERS, .github/PULL_REQUEST_TEMPLATE.md, .github/ISSUE_TEMPLATE/bug_report.md, .github/ISSUE_TEMPLATE/feature_request.md, CHANGELOG.md, README.md. Pousser ces changements sur la branche main.
