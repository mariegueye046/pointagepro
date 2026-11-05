# PointagePro

Web-based attendance and leave management system, built with PHP 8.2 (OOP, custom MVC, no framework) and PostgreSQL.

*Application web de gestion des présences et des congés, développée en PHP 8.2 (POO, MVC sans framework) avec PostgreSQL.*

---

## 🇬🇧 English

### Features

- **Authentication**: email and password login, role-based access (Admin, Manager, Employee), CSRF protection
- **Attendance**: check-in / check-out by QR code (one unique QR per employee) or manual entry by an admin or manager
- **Automatic status**: Present, Late or Absent
- **Live dashboard**: KPI cards (present, late, absent, on leave), today's check-ins, attendance chart by department, refreshed every 30 seconds
- **Employee management**: create, edit and deactivate employees, filters, pagination
- **Leave management**: request, approval or rejection workflow, email notifications
- **Reports**: Excel and PDF exports (attendance, monthly summary, leaves, late arrivals)

### Tech stack

- PHP 8.2 (OOP, MVC architecture)
- PostgreSQL, accessed with PDO prepared statements
- HTML, CSS, JavaScript, Tailwind CSS, Chart.js
- Composer (endroid/qr-code, PhpSpreadsheet, TCPDF)

### Installation

1. Clone the repository:
   `git clone https://github.com/mariegueye046/pointagepro.git`
2. Install dependencies: `composer install`
3. Copy the environment file and fill in your database credentials:
   `cp .env.example .env`
4. Create a PostgreSQL database, then run the migrations:
   `php migrate.php`
5. Serve the `public/` folder with Nginx or Apache (or `php -S localhost:8000 -t public`).

### Author

Marie Ivonne Gueye, junior full stack developer, Dakar, Senegal.
Developed as a team project with Telly Tech.

---

## 🇫🇷 Français

### Fonctionnalités

- **Authentification** : connexion par email et mot de passe, accès par rôle (Admin, Manager, Employé), protection CSRF
- **Pointage** : arrivée et départ par QR Code (un QR unique par employé) ou saisie manuelle par un admin ou un manager
- **Statut automatique** : Présent, Retard ou Absent
- **Dashboard en direct** : cartes d'indicateurs (présents, retardataires, absents, en congé), pointages du jour, graphique par département, actualisé toutes les 30 secondes
- **Gestion des employés** : création, modification et désactivation, filtres, pagination
- **Gestion des congés** : demande, validation ou rejet, notifications par email
- **Rapports** : exports Excel et PDF (pointages, synthèse mensuelle, congés, retards)

### Technologies

- PHP 8.2 (POO, architecture MVC)
- PostgreSQL, avec requêtes préparées PDO
- HTML, CSS, JavaScript, Tailwind CSS, Chart.js
- Composer (endroid/qr-code, PhpSpreadsheet, TCPDF)

### Installation

1. Cloner le dépôt :
   `git clone https://github.com/mariegueye046/pointagepro.git`
2. Installer les dépendances : `composer install`
3. Copier le fichier d'environnement et renseigner les accès à la base :
   `cp .env.example .env`
4. Créer une base PostgreSQL, puis lancer les migrations :
   `php migrate.php`
5. Servir le dossier `public/` avec Nginx ou Apache (ou `php -S localhost:8000 -t public`).

### Auteure

Marie Ivonne Gueye, développeuse full stack junior, Dakar, Sénégal.
Projet réalisé en équipe avec Telly Tech.
