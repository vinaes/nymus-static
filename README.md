# Nymus Static Config

Remote configuration for [Nymus](https://apps.apple.com/app/nymus) — offline AI chat for iOS.

This repository stores the model list that the app fetches at launch. Adding or updating models here makes them available to all users without an app update.

## How it works

The app sends a GET request to:

```
https://raw.githubusercontent.com/vinaes/nymus-static/main/v1/models.json
```

The response is an array of model objects with localized descriptions, download URLs, and file metadata. The app displays this list on the onboarding and model picker screens.

## Issues

If you found a bug, want a new model, or have a feature request — create an Issue using one of the tags below.

### [Model] — Model request or download problem

A model stopped downloading, or you'd like to see a new model added.

**Required info:**
- Model name and source (e.g. Hugging Face link)
- Why this model? (quality, size, language support, etc.)
- Have you tested this model locally? (LM Studio, llama.cpp, etc.)
- GGUF quantization (e.g. Q4_K_M, Q5_K_M)

### [Bug] — Bug report

Something isn't working as expected.

**Required info:**
- App version (Settings → About)
- Device model (e.g. iPhone 15 Pro)
- iOS version (e.g. iOS 18.3)
- Selected model (e.g. Qwen3 1.7B)
- Parameters (context size, temperature)
- Steps to reproduce

### [Feature] — Feature request

You have an idea for a new feature.

**Required info:**
- Description of the feature
- Why it would be useful

---

# Nymus Static Config (RU)

Удалённая конфигурация для [Nymus](https://apps.apple.com/app/nymus) — оффлайн AI-чат для iOS.

В этом репозитории хранится список моделей, который приложение загружает при запуске. Добавление или обновление моделей здесь делает их доступными для всех пользователей без обновления приложения.

## Как это работает

Приложение отправляет GET-запрос на:

```
https://raw.githubusercontent.com/vinaes/nymus-static/main/v1/models.json
```

Ответ — массив объектов моделей с локализованными описаниями, ссылками для скачивания и метаданными файлов. Приложение показывает этот список на экранах онбординга и выбора модели.

## Issues

Если нашли баг, хотите новую модель или есть идея — создайте Issue с одним из тегов ниже.

### [Model] — Запрос модели или проблема с загрузкой

Модель перестала загружаться, или хотите добавить новую.

**Обязательная информация:**
- Название модели и источник (например, ссылка на Hugging Face)
- Почему эта модель? (качество, размер, поддержка языков и т.д.)
- Тестировали ли вы эту модель локально? (LM Studio, llama.cpp и т.д.)
- Квантизация GGUF (например, Q4_K_M, Q5_K_M)

### [Bug] — Баг-репорт

Что-то работает не так.

**Обязательная информация:**
- Версия приложения (Настройки → О приложении)
- Модель устройства (например, iPhone 15 Pro)
- Версия iOS (например, iOS 18.3)
- Выбранная модель (например, Qwen3 1.7B)
- Параметры (размер контекста, температура)
- Шаги для воспроизведения

### [Feature] — Запрос фичи

У вас есть идея для новой функции.

**Обязательная информация:**
- Описание фичи
- Почему она была бы полезна
