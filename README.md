# 📚 StudyBox

Une plateforme web complète dédiée aux étudiants, centralisant tous les outils nécessaires à une étude efficace : cours, notes, planning, révision et chronomètre — dans une seule application.

## ✨ Fonctionnalités

| Module | Description |
|--------|-------------|
| 📁 **Modules** | Organiser ses cours par matière, uploader des documents (PDF, DOCX) |
| 📝 **Notes** | Éditeur de notes enrichi (gras, italique, souligné) avec Tiptap |
| 📅 **Planner** | Calendrier mensuel + timeline journalière + gestion des tâches |
| 🔁 **Révision** | Flashcards, Quiz, sessions de révision active avec mode Pomodoro |
| ⏱️ **Timer** | Chronomètre de sessions d'étude avec historique |
| 📊 **Dashboard** | Vue d'ensemble de la progression et des objectifs |
| 👤 **Profil** | Gestion du compte et des paramètres personnels |
| 🔐 **Auth** | Inscription, connexion, vérification par email, réinitialisation de mot de passe |

---

## 🛠️ Stack technique

### Frontend
- **React 19** + Vite
- **React Router** — navigation SPA
- **Tiptap** — éditeur de texte riche
- **Lucide React** — icônes
- CSS personnalisé + thème sombre

### Backend
- **NestJS** (Node.js + TypeScript)
- **TypeORM** + **MySQL**
- **Nodemailer** — envoi d'emails de vérification
- **Multer** — upload de fichiers
- **pdf-parse** + **Mammoth** — extraction de contenu depuis PDF et DOCX
- **Bcrypt** — hachage des mots de passe

---

## 🚀 Lancer le projet

### Prérequis
- Node.js ≥ 18
- MySQL

### Backend

```bash
cd backend
npm install
# Configurer les variables d'environnement (voir .env.example)
npm run start:dev
```

### Frontend

```bash
cd frontend
npm install
npm run dev
```

L'application sera accessible sur `http://localhost:5173`

---

## 📁 Structure du projet

```
StudyBox/
├── backend/
│   └── src/
│       ├── auth/          # Authentification & vérification email
│       ├── modules/       # Gestion des matières/cours
│       ├── notes/         # Notes étudiantes
│       ├── tasks/         # Tâches du planner
│       ├── timer/         # Sessions chronomètre
│       ├── progress/      # Objectifs & suivi
│       ├── documents/     # Upload et extraction de documents
│       └── revision/      # Flashcards, Quiz, sessions de révision
└── frontend/
    └── src/
        └── components/
            ├── Auth/      # Connexion, inscription, reset password
            ├── Dashboard/ # Page d'accueil
            ├── Module/    # Gestion des cours
            ├── Notes/     # Éditeur de notes
            ├── Planner/   # Calendrier & tâches
            ├── Revision/  # Flashcards, Quiz, Pomodoro
            └── Timer/     # Chronomètre d'étude
```

---

## 👩‍💻 Auteure

**Doha Saif** — Étudiante Ingénieur ILISI, FSTM Mohammedia  
📬 saifdoha71@gmail.com
