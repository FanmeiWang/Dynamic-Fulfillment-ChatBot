# Dynamic-Fulfillment-ChatBot
# Dynamic-Fulfillment-ChatBot

## Overview
This repository demonstrates a chatbot integration with Dialogflow using a Flask-based webhook. It highlights dynamic intent handling and personalized responses based on user input. The project serves as an educational example of a conversational AI implementation.

---

## Features
- **Dynamic Intent Fulfillment**:
  - Handles intents such as `AskHobbies` and `HobbyFollowUp`.
  - Suggests activities based on user hobbies with personalized responses.
- **Flask Webhook**:
  - Processes Dialogflow requests and responds dynamically.
- **Customizable Logic**:
  - Logic can be extended for new intents and responses.

---

## How It Works
1. **Dialogflow Intents**:
   - `AskHobbies`: Identifies hobbies like sports, music, or reading.
   - `HobbyFollowUp`: Responds to follow-up questions (e.g., "yes" or "no").
2. **Flask Routes**:
   - `/`: Returns a placeholder JSON with a student number for testing.
   - `/webhook`: Handles intents and processes requests from Dialogflow.
3. **Ngrok Integration**:
   - Exposes the Flask app for Dialogflow webhook integration.

---

## Example Interaction
### Intent: `AskHobbies`
- **User Input**: "I like basketball."
- **Bot Response**: "You seem to love sports! Have you tried exploring hiking trails or playing tennis with friends?"

### Intent: `HobbyFollowUp`
- **User Input**: "yes"
- **Bot Response**: "Great! Here are some more ideas for you to explore. Have fun!"

---

## Setup Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/Dynamic-Fulfillment-ChatBot.git
   cd Dynamic-Fulfillment-ChatBot

## Install dependencies:
pip install -r requirements.txt


## Add a .env file for sensitive variables: Create a .env file in the root directory with the following content:
STUDENT_NUMBER=your-student-number
NGROK_AUTH_TOKEN=your-ngrok-auth-token

## Run the Flask app:
python app.py


