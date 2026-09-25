# MLOps: развертывание и поддержка моделей машинного обучения

Учебный курс, 36 академических часов, 18 практических занятий (1 пара в неделю),
форма контроля — **зачёт** (конец декабря). Лекций нет: каждое занятие — работа за клавиатурой.

## Что студент получает на выходе

Один сквозной проект, который живёт весь семестр и к декабрю превращается
в полноценный ML-сервис:

> модель оттока клиентов → воспроизводимый пайплайн (DVC) → трекинг экспериментов (MLflow)
> → тесты и CI → REST-сервис (FastAPI) → контейнер (Docker) → локальный стенд (compose)
> → CD и публикация образа → мониторинг (Prometheus + Grafana + Evidently) → автопереобучение

Итоговый проект и есть допуск к зачёту.

## 🎓 Для студентов

**НАЧНИ ОТСЮДА:** [**HOW_TO_SUBMIT_LABS.md**](HOW_TO_SUBMIT_LABS.md) — полная инструкция как выполнять и сдавать лабы

Также полезно:
- [STUDENT_GIT_GUIDE.md](STUDENT_GIT_GUIDE.md) — полное руководство по Git
- [GIT_CHEATSHEET.md](GIT_CHEATSHEET.md) — краткая шпаргалка по Git
- [SETUP_BY_OS.md](SETUP_BY_OS.md) — установка Git для твоей ОС
- [docs/setup.md](docs/setup.md) — установка окружения Python

## Навигация

| Раздел | Что внутри |
|---|---|
| [docs/syllabus.md](docs/syllabus.md) | Тематический план всех 18 занятий |
| [docs/theory/](docs/theory/) | Теория курса: 9 конспектов вместо лекций |
| [docs/student-guide.md](docs/student-guide.md) | Памятка студента: что делать за семестр |
| [docs/announcement.md](docs/announcement.md) | Готовые тексты для рассылки группе |
| [docs/setup.md](docs/setup.md) | Установка окружения (Windows / macOS / Linux) |
| [docs/assessment.md](docs/assessment.md) | Зачёт: требования, критерии, чек-лист защиты |
| [bot/](bot/) | Телеграм-бот курса: выдаёт задания, принимает и проверяет работы |
| [lessons/](lessons/) | По папке на занятие: `handout.md` (задание для студента) |
| [template/](template/) | Стартовый скелет проекта — студенты клонируют его |
| [reference-project/](reference-project/) | Эталонное решение целиком — ответ преподавателя |

## Стек

Python 3.11 · Git · pre-commit + ruff · DVC · MLflow · pytest · GitHub Actions ·
FastAPI · Docker + docker-compose · MinIO · Prometheus + Grafana · Evidently · Prefect

Всё open-source, ставится локально, работает без облачного бюджета.

## Как пользоваться репозиторием преподавателю

1. Перед семестром: пройти [docs/setup.md](docs/setup.md) на машине аудитории, прогнать
   `reference-project/` целиком (`make all`) — это проверка, что стенд жив.
2. Перед парой: прочитать `lessons/NN-*/plan.md` (там тайминг, демо-скрипт и типовые ошибки).
3. Материалы студентам раздаёт бот: `/theory N` — конспект к занятию,
   `/task N` — методичка и список «что сдать».
4. ДЗ принимает бот (`/submit N`), сводка — `/report N`, ведомость — `/export`.
   Подробно: [docs/workflow.md](docs/workflow.md).

## Проверка проекта одной командой

Тот же чек-лист, что у бота, работает из терминала — и у преподавателя,
и у студента:

```bash
python -m bot.checker --path .                    # все занятия
python -m bot.checker --path . --lesson 11        # одно занятие
python -m bot.checker --repo <url> --lesson 9 --gh
```
