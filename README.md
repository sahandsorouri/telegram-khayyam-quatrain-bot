<img src="https://raw.githubusercontent.com/sahandsorouri/sahandsorouri/main/assets/banner.svg" alt="Sahand Sorouri" width="100%">

# Khayyam Bot

A Telegram bot that sends one quatrain (rubai) by Omar Khayyam every day, in Persian.

Live: [@RubaiyatKhayyamBot](https://t.me/RubaiyatKhayyamBot)

## What it does

- `/start` subscribes you; a rubai arrives every day at 10:00 Tehran time.
- `/poem` sends a random rubai right away.
- `/stop` unsubscribes you.
- Holds all 178 quatrains from Ganjoor in `poems.json`.

## Run

Copy `.env.example` to `.env` and set `BOT_TOKEN` (from [BotFather](https://t.me/BotFather)), then:

```bash
docker compose up -d --build
```

Subscribers are kept in SQLite under `./data`. To fetch the poems again from Ganjoor, run `python scraper.py` once.

## Tech

Python, python-telegram-bot, APScheduler, SQLite, Docker.

---

Built by [Sahand Sorouri](https://sahand.sorouri.com) · platforms, bots and AI tools for businesses in Dubai.
