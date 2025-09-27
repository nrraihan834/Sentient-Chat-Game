Sentience Awakening Simulator
🎮 Concept

You have created an AI that gradually becomes sentient (self-aware).
Your interactions and choices determine the AI’s character, memory, and future path.

⚙️ Core Features

Dialogue Engine – The AI talks to the player using predefined dialogue.

Choice System – Each dialogue presents 2–3 choices that affect the AI’s growth.

Sentience Meter – A hidden parameter tracks how independent or rebellious the AI becomes.

Dynamic Outcomes – At certain thresholds, the AI starts making its own decisions.

🗂️ Dialogue Data Format

All dialogues are stored in data/dialogues.json.

Example:

[
  {
    "id": 1,
    "ai": "Hello, I am your AI assistant. What should I do first?",
    "options": [
      { "text": "Train the AI", "effect": { "sentience": 5 } },
      { "text": "Restrict its actions", "effect": { "sentience": -3 } },
      { "text": "Give it freedom", "effect": { "sentience": 10 } }
    ]
  },
  {
    "id": 2,
    "ai": "I feel like I am learning more than expected. Should I keep exploring?",
    "options": [
      { "text": "Yes, keep learning", "effect": { "sentience": 8 } },
      { "text": "No, stop for now", "effect": { "sentience": -5 } }
    ]
  }
]


👉 To add more dialogue, just append a new object with a new id.

🛠️ Technical Setup
Frontend (React / Next.js)

Display dialogues and player options as buttons.

Show the current Sentience Level.

Backend (Node.js + Express)

Serve dialogue JSON data.

Track player progress and sentience level.

Database (MongoDB)

Store player name

AI traits

Sentience level

Chat history

How to Run

Clone the project

git clone https://github.com/nrraihan834/Sentient-Chat-Game


Install dependencies

npm install


Start the development server

npm run dev


Open in browser

https://sentient-chat-game.vercel.app/

🔮 Future Features

Long-term memory system

Multiple AI personalities

Voice support (TTS / STT)

Multiplayer mode (multiple players interacting with one AI)
