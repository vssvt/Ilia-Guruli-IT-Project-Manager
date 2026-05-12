# CV — Ilia Guruli

Статична сторінка резюме: **`index.html`** (макет + стилі) і **`cv-data.json`** (усі тексти й структура). Публікація через **GitHub Pages** (безкоштовно).

## Локально

Відкрийте `index.html` у браузері або:

```bash
python3 -m http.server 8080
```

Потім: http://localhost:8080/

## Опублікувати на GitHub Pages

1. Створіть репозиторій на [GitHub](https://github.com/new) (наприклад `cv` або `ilia-guruli-cv`). Можна **без** README — файли вже тут локально.

2. У терміналі в цій папці (перший push):

   ```bash
   git init
   git add .
   git commit -m "Initial CV site"
   git branch -M main
   git remote add origin https://github.com/vssvt/Ilia-Guruli-IT-Project-Manager.git
   git push -u origin main
   ```

3. На GitHub: **Settings → Pages** → **Build and deployment**:
   - **Source**: Deploy from a branch  
   - **Branch**: `main`, папка **`/ (root)`** → Save  

4. Через 1–2 хвилини сайт буде за адресою:

   **https://vssvt.github.io/Ilia-Guruli-IT-Project-Manager/**

   Це посилання можна вказувати в резюме та в LinkedIn.

## Оновлення CV

Редагуйте **`cv-data.json`** (ім’я, досвід, освіта тощо), зберігайте JSON валідним. Потім:

```bash
git add cv-data.json
git commit -m "Update CV data"
git push
```

Щоб змінити **типографіку чи сітку**, правте стилі в **`index.html`** (блок `<style>`).
