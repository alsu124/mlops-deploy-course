# 📝 Как выполнять и сдавать лабы

Этот файл - полная инструкция для студентов как работать с первой лабой и всеми остальными.

---

## 🎯 ОБЩИЙ ПРОЦЕСС

### Шаг 1: Создай свой репо на GitHub

1. Открой https://github.com/new
2. Имя репо: `mlops-ТВОЯ_ФАМИЛИЯ` (пример: `mlops-ivanov`)
3. Нажми "Create repository"

### Шаг 2: Клонируй курс репо

```bash
git clone https://github.com/alsu124/mlops-deploy-course.git
cd mlops-deploy-course
```

### Шаг 3: Добавь свой репо как remote

```bash
git remote add origin https://github.com/ТВОЙ_НИК/mlops-ФАМИЛИЯ.git
```

Проверка:
```bash
git remote -v
# origin     https://github.com/ТВОЙ_НИК/mlops-ФАМИЛИЯ.git
# upstream   https://github.com/alsu124/mlops-deploy-course.git
```

### Шаг 4: Создай ветку для ДЗ

```bash
git checkout -b lesson-01-solution
```

### Шаг 5: Выполни задание

Открой `lessons/01-intro-project-setup/handout.md` и следуй инструкциям

### Шаг 6: Коммитьте свою работу

```bash
git add .
git commit -m "ДЗ 1: описание что ты сделал"
```

### Шаг 7: Загрузи на свой GitHub

```bash
git push -u origin lesson-01-solution
```

### Шаг 8: Создай Pull Request

1. Открой https://github.com/alsu124/mlops-deploy-course
2. Нажми "Pull requests" (вверху)
3. Нажми "New pull request"
4. Выбери:
   - **base:** `alsu124/mlops-deploy-course` `main`
   - **compare:** `ТВОЙ_НИК/mlops-ФАМИЛИЯ` `lesson-01-solution`
5. Напиши описание что ты сделал
6. Нажми "Create pull request"

---

## 📚 ДЛЯ КАЖДОЙ ЛАБЫ

**Структура папки каждого занятия:**

```
lessons/01-intro-project-setup/
└── handout.md          ← ТВОЯ РАБОТА ЗДЕСЬ
                           Полное описание что делать
                           Все требования
                           Как проверить результат
```

**Что делать:**

1. Открой `lessons/NN-*/handout.md`
2. Прочитай требования
3. Выполни все шаги
4. Коммитьте и создай PR

---

## ✅ ПЕРВАЯ ЛАБА: БЫСТРЫЙ СТАРТ

```bash
# 1. Перейди в папку курса
cd ~/Desktop/mlops-homework

# 2. Создай ветку
git checkout -b lesson-01-solution

# 3. Открой задание
cat lessons/01-intro-project-setup/handout.md

# 4. Выполни все 5 шагов из handout.md

# 5. Коммитьте
git add .
git commit -m "ДЗ 1: Выполнена"

# 6. Пушь
git push origin lesson-01-solution

# 7. Создай PR на GitHub
```

---

## 🎓 НАВИГАЦИЯ ПО КУРСУ

| Лаба | Название | Папка |
|------|----------|-------|
| 1 | Введение. Окружение | `lessons/01-intro-project-setup/handout.md` |
| 2 | Git workflow | `lessons/02-git-workflow/handout.md` |
| 3 | Конфигурация и детерминизм | `lessons/03-config-and-determinism/handout.md` |
| 4 | Версионирование данных (DVC) | `lessons/04-dvc-data-versioning/handout.md` |
| ... | ... | ... |

Все остальные в папке `lessons/`

---

## 📞 ВОПРОСЫ?

1. **Как смотреть что нужно делать?**
   - Открой `lessons/NN-*/handout.md`

2. **Как запустить код?**
   - Следуй инструкциям в handout.md
   - Там все команды написаны

3. **Как проверить что работает?**
   - В handout.md есть чек-лист проверки

4. **Как сдать?**
   - Коммит → Push → Pull Request

---

## 🚀 ГОТОВ К НАЧАЛУ?

Начни со **Шага 1** выше и выполни первую лабу!

Удачи! 💪
