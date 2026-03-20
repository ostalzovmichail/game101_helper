
* [English](#english-version)
* [Русский](#russian-version)

<a name="english-version"></a>
# Account Entry (Game 101)

A Flutter app to manage players and track scores for the "Game 101" card game.

## Features
- Create and delete players (up to 6 players).
- Start a game when at least 2 players exist.
- Track each player’s score and update it during the game.
- Round counter with a "finish round" action.
- Reset all scores to zero when the game ends.
- Local persistence using SQLite (sqflite).
- English and Russian UI strings.

## Game Rules Implemented
- If a player’s score reaches 100, it is set to 50.
- If a player’s score reaches 101, it is reset to 0.
- If a player’s score is greater than 101, the UI shows a loss state for that player.

## Tech Stack
- Flutter / Dart
- Provider (state management)
- sqflite (SQLite storage)
- intl (localization)

## Run Locally
1. Install Flutter SDK.
2. Fetch dependencies:
   flutter pub get
3. Run the app:
   flutter run

## Project Structure (high level)
- lib/ui: UI pages and widgets
- lib/repository, lib/service: data access and state
- lib/db: SQLite helper
- lib/l10n: localization strings

<a name="russian-version"></a>
# Account Entry (Игра 101)

Flutter-приложение для ведения списка игроков и подсчёта очков в карточной игре «101».


## Возможности
- Добавление и удаление игроков (до 6 человек).
- Старт игры доступен при наличии минимум 2 игроков.
- Учёт очков каждого игрока и их изменение во время игры.
- Счётчик раундов и действие «завершить раунд».
- Сброс всех очков при завершении игры.
- Локальное хранение данных в SQLite (sqflite).
- Интерфейс на русском и английском языках.

## Реализованные правила
- При достижении 100 очков значение сбрасывается на 50.
- При достижении 101 очка значение сбрасывается на 0.
- Если очков больше 101, в интерфейсе показывается состояние проигрыша.

## Технологии
- Flutter / Dart
- Provider (управление состоянием)
- sqflite (SQLite)
- intl (локализация)

## Запуск
1. Установите Flutter SDK.
2. Установите зависимости:
   flutter pub get
3. Запустите приложение:
   flutter run

## Структура проекта (вкратце)
- lib/ui: экраны и виджеты
- lib/repository, lib/service: работа с данными и состоянием
- lib/db: помощник SQLite
- lib/l10n: строки локализации
