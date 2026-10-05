# Carnet de rechargement

Application de suivi de rechargement de cartouches, packagée en application Android (APK) via Capacitor et GitHub Actions.

- `www/index.html` — l'application (une seule page, tout est inclus).
- `package.json`, `capacitor.config.json` — configuration Capacitor.
- `.github/workflows/creer-cle.yml` — fabrique la clé de signature Android (une seule fois).
- `.github/workflows/apk-android.yml` — fabrique l'APK signé, à chaque nouvelle version.

Guide pas à pas complet : voir l'artifact « APK Carnet de rechargement pas à pas ».

Pour mettre à jour l'application, modifiez `www/index.html` (ou remplacez-le), changez `"version"` dans `package.json` si vous voulez, puis relancez le workflow **APK Android** dans l'onglet Actions du dépôt.
