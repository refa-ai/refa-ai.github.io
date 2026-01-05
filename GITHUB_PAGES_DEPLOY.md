# Инструкция по деплою на GitHub Pages

## ✅ Файлы готовы

Все HTML файлы скопированы в репозиторий:
- terms.html
- privacy.html
- refund.html
- pricing.html

## 🚀 Деплой

### Шаг 1: Закоммитить и запушить

```bash
cd /data/refa-ai.github.io
git add *.html README.md .gitignore
git commit -m "Add Paddle pages (terms, privacy, refund, pricing)"
git branch -M main
git push -u origin main
```

### Шаг 2: Настроить GitHub Pages

1. Зайдите на https://github.com/refa-ai/refa-ai.github.io
2. Settings → Pages
3. В разделе "Build and deployment":
   - **Source:** "Deploy from a branch"
   - **Branch:** `main`
   - **Folder:** `/ (root)`
4. Нажмите **Save**

### Шаг 3: Подождать несколько минут

GitHub Pages автоматически задеплоит сайт через 1-2 минуты.

## 🔗 URL для Paddle

После деплоя используйте эти URL в форме регистрации Paddle:

- **Web domains:** `https://refa-ai.github.io`
- **Pricing page:** `https://refa-ai.github.io/pricing.html`
- **Terms of service:** `https://refa-ai.github.io/terms.html` ⚠️ ОБЯЗАТЕЛЬНО
- **Privacy policy:** `https://refa-ai.github.io/privacy.html`
- **Refund policy:** `https://refa-ai.github.io/refund.html`

## ✅ Проверка

Откройте в браузере:
- https://refa-ai.github.io/terms.html
- https://refa-ai.github.io/pricing.html

Все должно работать!
