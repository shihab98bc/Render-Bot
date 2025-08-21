# Telegram Bot Deployment on Render

This is a Telegram bot that provides various services including number distribution, file submission, fake name generation, and 2FA code generation.

## Features

- Number distribution system with categories and sub-categories
- File submission system with Excel file processing
- Fake name generation with gender selection
- 2FA code generation with secret key storage
- Admin panel for managing users, buttons, and files
- Daily automated file merging and reporting
- Broadcast messaging to all users

## Deployment on Render

1. Fork this repository to your GitHub account
2. Create a new Web Service on Render and connect your GitHub repository
3. Add the following environment variables in Render:
   - `BOT_TOKEN`: Your Telegram bot token from @BotFather
   - `ADMIN_IDS`: Comma-separated list of admin user IDs (e.g., "5705479420,123456789")
   - `SUPPORT_USERNAME`: Your support Telegram username (e.g., "@shihab98bc")
4. Deploy the application

## Local Development

1. Clone the repository
2. Install dependencies: `pip install -r requirements.txt`
3. Set up environment variables or create a `config.json` file
4. Run the bot: `python bot.py`

## File Structure

- `bot.py`: Main bot application
- `config.json`: Configuration file (optional if using environment variables)
- `data.json`: Data storage file
- `requirements.txt`: Python dependencies
- `Procfile`: Render process definition
- `.render.yaml`: Render deployment configuration
- `uploads/`: Directory for uploaded files
- `uploads/user_files/`: Directory for user-submitted files