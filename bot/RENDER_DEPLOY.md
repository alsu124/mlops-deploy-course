# 🚀 RENDER DEPLOYMENT - ПОЛНОСТЬЮ БЕСПЛАТНО

Render - это бесплатная альтернатива Railway. БОТ РАБОТАЕТ 24/7 БЕЗ ОПЛАТЫ!

---

## ✅ БЫСТРЫЙ СТАРТ (5 МИНУТ)

### 1️⃣ Зарегистрируйся на Render

Перейди: https://render.com

Нажми **"Sign up"** → выбери **"Continue with GitHub"** → залогинься

### 2️⃣ Создай новый сервис

- Нажми **"+ New"** → выбери **"Web Service"**
- Выбери **"Deploy an existing GitHub repo"**
- Разреши доступ Render к твоим репо
- Выбери репо: **`alsu124/mlops-deploy-course`**

### 3️⃣ Настрой сервис

**Заполни форму:**

| Поле | Значение |
|------|----------|
| Name | `mlops-bot` |
| Environment | `Python 3` |
| Build Command | `pip install -r requirements.txt` |
| Start Command | `python3 bot/telegram_bot.py` |
| Free tier | ✅ Выбери (бесплатно) |

### 4️⃣ Добавь переменную BOT_TOKEN

Нажми **"Advanced"** → **"Add Environment Variable"**:

```
Key: BOT_TOKEN
Value: 8635163294:AAHHIMy1Sj3vtl9Arst8Rlk8_SnXvBDjTaY
```

### 5️⃣ Deploy!

Нажми **"Create Web Service"**

Render начнет развертывание. Подожди 3-5 минут.

---

## ✅ ПРОВЕРКА

1. В Render Dashboard смотри логи
2. Когда статус станет **"live"** (зеленый) - бот работает!
3. Открой Telegram → @Mlopsitisbot → /start

**Если меню показалось - УРА!** ✅

---

## 🎯 ПЛЮСЫ RENDER

✅ 100% бесплатно (даже без карточки)  
✅ Бот работает 24/7  
✅ Автоматический перезапуск  
✅ Встроенные логи  
✅ Просто развертывается  

---

## 📊 СРАВНЕНИЕ

| Сервис | Цена | Работает 24/7 | Бесплатно |
|--------|------|---------------|-----------|
| Render | Бесплатно | ✅ Да | ✅ Да |
| Railway | Trial закончен | ❌ Требует оплата | ❌ Нет |
| TimeWeb | Платно | ❌ Проблемы сети | ❌ Нет |
| Heroku | Платно | ❌ Требует оплата | ❌ Нет |

---

## 🚀 НАЧИНАЙ!

1. Открой https://render.com
2. Залогинься через GitHub
3. Create Web Service
4. Выбери mlops-deploy-course
5. Добавь BOT_TOKEN
6. Deploy!

**Готово! БОТ РАБОТАЕТ! 🎉**

---

Если нужна помощь - напиши!
