# Telegram_weatherBot
The repository details the implementation of a Telegram bot that provides weather-related information regarding the place specified by the user. It works by utilizing the OpenWeather API to get current weather details of the concerned location

## Overview
Telegram Weather Bot is a Python-based chatbot designed to provide current weather information using the Telegram API and OpenWeatherMap API. Users can inquire about the weather in predefined cities or share their location for real-time weather updates.

## Prerequisites
Before building the project, ensure you have the following:
- Basic knowledge of Python
- Telegram Account
- OpenWeather Account

## Step 1: Get API Credentials
1. Go to [web.telegram.org](https://web.telegram.org/) and initiate a chat with BotFather.
2. Send the command `/newbot` to BotFather.
3. Choose a name for your bot (e.g., "yourWeatherBot") and a username ending in "bot" (e.g.,"weather_bot").
4. BotFather will provide a token (API key for Telegram). Keep it secure.

## Step 2: Obtain OpenWeatherMap API Key
1. Sign up at [OpenWeatherMap](https://openweathermap.org/) and verify your email.
2. Log in to your OpenWeatherMap account.
3. Navigate to the "API Keys" section and copy your API key.

## Step 3: Code Setup

### Installation
1. Install the required dependency:
   
    python3 -m pip install requests
    

### Getting Started
1. Create a new Python file, e.g., `telegram.py`, and open it in your preferred editor.
2. Copy and paste the provided Python code into `telegram.py`.

### Define Functions
1. Define Lambda functions for parsing updates from Telegram and weather responses.
2. Implement functions for configuring logging, parsing configuration, making requests, getting updates, and building keyboards.
3. Add functions for querying OpenWeatherMap for weather, sending messages to chat, and getting the last update ID.

### Main Functionality
1. Keep track of conversation states with a dictionary (`chats`).
2. Implement the `handleUpdates` function to process incoming messages.
3. Create the main loop in the `main` function to continuously poll for updates and handle them.

### Cities and API Keys
- Predefined cities in the code: Thiruvananthapuram, Delhi, Bengaluru, Pune, Cochin.
- Ensure to replace placeholders in the code with your API keys for Telegram and OpenWeatherMap.

### Testing
1. Run the script in your terminal:
   
    python3 telegram.py
  
2. Open your Telegram app and search for the bot using the chosen username.
3. Send the command `/weather` to initiate the weather inquiry.
4. Select a predefined city or share your location to receive current weather details.


