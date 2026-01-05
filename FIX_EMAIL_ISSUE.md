# Решение проблемы с приватным email

## ❌ Ошибка

```
remote: error: GH007: Your push would publish a private email address.
push declined due to email privacy restrictions
```

## ✅ Решение

### Вариант 1: Использовать GitHub no-reply email (уже применено)

```bash
cd /data/refa-ai.github.io
git config user.email "refa-ai@users.noreply.github.com"
git config user.name "refa-ai"
git commit --amend --reset-author --no-edit
git push -u origin main
```

### Вариант 2: Сделать email публичным

1. Зайдите на https://github.com/settings/emails
2. Снимите галочку "Keep my email addresses private"
3. Или добавьте email в "Public email addresses"
4. Попробуйте push снова

### Вариант 3: Использовать другой email

```bash
cd /data/refa-ai.github.io
git config user.email "your-public-email@example.com"
git commit --amend --reset-author --no-edit
git push -u origin main
```

## 📝 После исправления

После успешного push:
1. Настройте GitHub Pages (Settings → Pages)
2. Сайт будет доступен через 1-2 минуты

