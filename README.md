# Dynamic-Fulfillment-ChatBot
author @ Fanmei Wang

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

