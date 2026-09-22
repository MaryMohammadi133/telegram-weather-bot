# Telegram Weather Bot 🌤️

A Python practice project that uses the OpenWeather API to provide weather information through a Telegram bot.

## Features

- Current temperature in Celsius
- Current humidity
- Estimated temperature range for the rest of today
- Tomorrow's forecast, including the temperature near noon
- Estimated minimum and maximum temperatures from forecast samples
- Support for English city names and selected Persian city names
- Error handling for unknown cities, connection issues, and API errors

## Technologies

- Python
- python-telegram-bot
- httpx
- OpenWeather API
- Google Colab

## How to Run

1. Open `wheatherforcasting.ipynb` in Google Colab.
2. Create a Telegram bot using @BotFather and obtain its token.
3. Obtain an API key from OpenWeather.
4. Add these two secrets in Google Colab and enable notebook access:
   - `TELEGRAM_BOT_TOKEN`
   - `WEATHER_API_KEY`
5. Run the installation cell.
6. Run the main bot cell.
7. Open your bot in Telegram, send `/start`, and enter a city name.

Examples: `Rasht,IR`, `London,GB`, or `رشت`.

## Notes

- API keys are read from Colab Secrets and are not included in the notebook.
- Forecast ranges are calculated from three-hour samples, so they are not exact daily minimum and maximum temperatures.
- Today's range covers the remaining hours of the day, not the entire day.
- The bot runs while the Colab session and bot cell remain active. This setup does not provide 24/7 hosting.
- Bot replies are in Persian.

## Learning Goals

Practice working with APIs, asynchronous Python, Telegram message handlers, JSON responses, and error handling.
