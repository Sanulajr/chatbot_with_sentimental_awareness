# Sentiment Chatbot

This is a simple sentiment analysis chatbot built using Python and the `TextBlob` library. The bot analyzes the sentiment of user input and responds with appropriate messages based on the sentiment score.

## Project Overview

The chatbot uses **TextBlob** to analyze the sentiment of the input text. It provides responses that reflect different emotional states based on the sentiment polarity score. The sentiment ranges from -1 (very negative) to 1 (very positive), and based on this, the bot replies with a tailored message. It can respond to happy, neutral, sad, and very sad moods.

### Features

- **Sentiment Analysis**: Analyzes the sentiment of the user's input and provides a corresponding response.
- **Friendly and Supportive Responses**: The bot responds positively to happy input and offers comfort for negative or sad input.
- **User Interaction**: Users can interact with the chatbot by typing in their mood or thoughts. They can type 'exit' to quit the chat.
  
## Technologies Used

- **Python**: The programming language used for implementing the chatbot logic.
- **TextBlob**: A Python library used for performing sentiment analysis on text.

## How It Works

1. The user enters text.
2. The `TextBlob` library analyzes the text and computes a sentiment score.
3. Based on the sentiment score, the bot determines the user's mood:
   - **Very Happy**: Sentiment score > 0.5
   - **Happy**: Sentiment score between 0.1 and 0.5
   - **Sad**: Sentiment score between -0.1 and -0.5
   - **Very Sad**: Sentiment score < -0.5
   - **Neutral**: Sentiment score between -0.1 and 0.1
4. The bot responds with a personalized message based on the detected mood.

## Usage

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/your-username/sentiment-chatbot.git
   ```

2. Install the required dependencies:

   ```bash
   pip install textblob
   ```

3. Run the chatbot:

   ```bash
   python sentiment_chatbot.py
   ```

4. Type your thoughts or feelings into the terminal. The bot will respond based on the sentiment of your input.

5. Type `exit` to quit the chatbot.

## Example

```bash
Welcome to the Sentiment Chatbot! Type 'exit' to quit.
Enter text: I'm feeling awesome today!
Sentiment: 0.80
Response: Wow, you're on cloud nine! Keep shining and spreading those positive vibes. 😊🌟 Everything looks brighter when you're this happy!
```

## Future Improvements

- Implementing a more advanced sentiment analysis model for better accuracy.
- Allowing the bot to recognize more complex moods and provide more nuanced responses.
- Adding a graphical user interface (GUI) to make the bot more user-friendly.
