# RPL — Role Playing Life

**Игровое зеркало реальной жизни**: персонаж обновляется из реальных данных и рефлексии; фокус на консистентности выбранного вектора, а не на «стань лучше».

## Документы

### Universal System Layer

Эти документы должны оставаться обезличенными и переиспользуемыми.

| Файл | Описание |
|------|----------|
| [RPL-CONCEPT.md](RPL-CONCEPT.md) | **Канон** — полная концепция продукта |
| [SOURCES.md](SOURCES.md) | Связь с сырыми источниками (транскрипты, Inbox) |
| [RPL-HARNESS.md](RPL-HARNESS.md) | Операционная система RPL из ролей, памяти, ритуалов и скиллов |
| [RPL-DATA-BOUNDARIES.md](RPL-DATA-BOUNDARIES.md) | Границы между системными правилами, пользовательскими данными и обезличенными паттернами |
| [RPL-ONBOARDING-RITUALS.md](RPL-ONBOARDING-RITUALS.md) | Онбординг, ритуалы, правила памяти и критерии хороших квестов |
| [RPL-LIFE-COMPASS.md](RPL-LIFE-COMPASS.md) | Универсальная диагностика баланса и направления жизни для RPL Harness |
| [RPL-HUMAN-JOURNEY.md](RPL-HUMAN-JOURNEY.md) | Путь человека через RPL: инструменты, практики, поддержка, книги и фильмы |
| [RPL-GIT-DISTRIBUTION.md](RPL-GIT-DISTRIBUTION.md) | Как раздавать RPL Harness через Git без личных данных |

### Public Skills And Templates

Эти папки проектируются как будущий публичный пакет RPL Harness.

| Путь | Описание |
|------|----------|
| [skills/](skills/) | Codex-style skills: онбординг, зеркала, квесты, Life Compass, Freedom Number, оффер и куратор памяти |
| [templates/](templates/) | Шаблоны приватного пользовательского сейва без реальных личных данных |

### Private User Instance

Реальные пользовательские сейвы являются приватным слоем и не должны попадать в публичный Harness без явного обезличивания.

Рекомендуемая структура приватного сейва:

```text
USER/
  USER-MEMORY.md
  USER-PROFILE.md
  USER-FUTURE-{horizon}.md
  USER-LIFE-COMPASS.md
  USER-GAP-{horizon}.md
  USER-QUESTS.md
  USER-WEEKLY-MIRROR.md
  USER-EVIDENCE-LOG.md
  assets/
```

> Перед публикацией в Git пользовательский слой должен быть исключен. См. [.gitignore](.gitignore) и [RPL-GIT-DISTRIBUTION.md](RPL-GIT-DISTRIBUTION.md).

## Пересечения с другими проектами

- Тема «жизнь как игра / коуч / дневник прогресса» в голосовой заметке см. [SOURCES.md](SOURCES.md) и [collective-open-platform](../collective-open-platform/README.md) — разные оси (психология+продукт vs платформа разработки).

## Навигация

- [Все проекты](../README.md) · [Корень](../../README.md) · [CLOUD.md](../../CLOUD.md)
