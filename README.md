# Advanced Telegram Bot on GitHub Pages

## 🤖 Project Overview

This is an advanced Telegram bot hosted on GitHub Pages, featuring multiple interactive commands and a responsive web interface.

## ✨ Features

- 🚀 Multiple Interactive Commands
  - `/start`: Bot initialization
  - `/help`: List available commands
  - `/echo`: Repeat your message
  - `/weather`: Get current weather for a city
  - `/quote`: Retrieve a random inspirational quote
  - `/calc`: Perform mathematical calculations

- 📊 Advanced Logging System
  - Timestamped log entries
  - Color-coded logs
  - Scrollable log display

- 🎨 Responsive Web Design
  - Modern, clean user interface
  - Mobile-friendly layout
  - Customizable color scheme

## 🛠️ Prerequisites

- GitHub account
- Telegram account
- Telegram Bot created via BotFather
- (Optional) OpenWeatherMap API key for weather feature

## 🚀 Setup Instructions

### 1. Create Telegram Bot

1. Open Telegram and search for `@BotFather`
2. Send `/newbot` and follow instructions
3. Receive your bot token

### 2. Configure Project

1. Clone this repository
2. Open `index.html`
3. Locate the `CONFIG` object in the script
4. Replace placeholders:
   ```javascript
   const CONFIG = {
     BOT_TOKEN: 'your_telegram_bot_token_here',
     WEATHER_API_KEY: 'optional_openweathermap_api_key',
     WEBHOOK_URL: window.location.origin
   };
   ```

### 3. Deploy to GitHub Pages

1. Create a new GitHub repository
2. Push your files to the repository
3. Go to repository Settings > Pages
4. Select the main branch
5. Your site will be published at `https://yourusername.github.io/repository-name/`

## 🔒 Security Notes

- Never share your bot token publicly
- Use environment variables or secure methods to manage tokens
- Be cautious with the `/calc` command's `eval()` function

## 🛠 Customization

### Styling
- Modify CSS variables in `:root` to change color scheme
- Adjust `style` tag for further customizations

### Commands
- Edit `commands` object in the `TelegramBot` class
- Add new command handlers as needed

## 📦 Dependencies

- No external library dependencies
- Uses native JavaScript
- Optional external APIs
