✒ Correspond — Multi-Provider AI Chat

A simple, modern AI chat interface built with HTML, CSS, and JavaScript.

Correspond allows you to select an AI provider, enter its API key, select a model, and send messages directly from the browser.

---

✨ Features

- Multi-provider AI chat
- Provider selection
- Model selection
- API key input
- Chat history during the current page session
- User and AI message bubbles
- Typing indicator
- Animated UI
- Responsive design
- Dark glass-style interface
- Enter to send messages
- Shift + Enter for a new line
- Clear chat history
- API key is kept in JavaScript memory
- No database required
- No Python required

---

🤖 Supported AI Providers

The code currently contains these providers:

Provider| API Type
Groq| OpenAI-compatible
Google Gemini| Gemini API
OpenAI| OpenAI-compatible
OpenRouter| OpenAI-compatible
Together AI| OpenAI-compatible
Mistral| OpenAI-compatible
Cohere| Cohere API

---

🖼️ Provider Logos

The interface can use provider logos from Simple Icons:

Groq

https://cdn.simpleicons.org/groq

Google Gemini

https://cdn.simpleicons.org/googlegemini

OpenAI

https://cdn.simpleicons.org/openai

OpenRouter

https://cdn.simpleicons.org/openrouter

Together AI

https://cdn.simpleicons.org/together

Mistral AI

https://cdn.simpleicons.org/mistralai

Cohere

https://cdn.simpleicons.org/cohere

---

🧠 Models Included in the Code

The following model names are configured in the "PROVIDERS" object of the provided code.

Groq

llama-3.3-70b-versatile

---

Google Gemini

gemini-2.0-flash

---

OpenAI

gpt-4o-mini

---

OpenRouter

meta-llama/llama-3.1-8b-instruct:free

---

Together AI

meta-llama/Llama-3.3-70B-Instruct-Turbo-Free

---

Mistral AI

mistral-small-latest

---

Cohere

command-r-08-2024

«These are the model IDs configured in this project. The project does not automatically retrieve a provider's current model list.»

---

📁 Project Structure

The project can be kept as a single HTML file.

Correspond/
└── index.html

The HTML file contains:

HTML
CSS
JavaScript

There is no separate Python application.

---

🚀 Running the Project

The project can be served using a PHP development server.

1. Install PHP

Make sure PHP is installed on your system.

Check:

php --version

---

2. Open the project directory

Example:

cd /path/to/Correspond

---

3. Start the PHP server

php -S localhost:8000

The server will start on:

http://localhost:8000

Open that address in your browser.

---

📱 Running in Termux

If PHP is installed in Termux:

php --version

Go to the folder containing the HTML file:

cd /path/to/Correspond

Start the PHP server:

php -S 0.0.0.0:8000

Then open:

http://localhost:8000

on the same device.

---

🔑 API Key

The application asks for an API key when you select a provider.

The key is stored in the JavaScript variable:

apiKey

It is used by the browser when making the API request.

The provided code does not save the API key to:

localStorage
sessionStorage
IndexedDB
cookies

The key therefore exists only in the current JavaScript runtime.

---

🔄 How the Application Works

The basic flow is:

Open index.html
       ↓
Select AI provider
       ↓
Select model
       ↓
Enter API key
       ↓
Enter message
       ↓
JavaScript creates API request
       ↓
fetch()
       ↓
Selected AI provider
       ↓
AI response
       ↓
Response displayed in chat

---

🧩 Provider Configuration

The providers are stored inside:

PROVIDERS

The provider order is controlled by:

PROVIDER_ORDER

The application uses the selected provider to determine:

- API endpoint
- API type
- available models
- request format
- response format

---

📡 API Requests

Most providers in the code use an OpenAI-compatible chat completion format.

The following providers use this format:

Groq
OpenAI
OpenRouter
Together AI
Mistral

The code sends requests using:

fetch()

---

Google Gemini

Gemini uses its own request format.

The application sends a request to:

generativelanguage.googleapis.com

using the selected Gemini model and API key.

---

Cohere

Cohere uses its own API request and response handling.

The code sends the request to:

api.cohere.com

---

💬 Chat History

Messages are stored in the JavaScript variable:

history

The history is used when sending subsequent messages so the conversation can continue.

Example structure:

User message
      ↓
AI response
      ↓
history
      ↓
Next API request

The history exists only while the page is running.

Refreshing the page clears the current conversation.

---

🧹 Clear Chat

The interface includes a clear-chat function.

When the chat is cleared, the current JavaScript conversation history is removed and the chat interface is reset.

---

⌨️ Keyboard Controls

Enter

Press:

Enter

to send a message.

New Line

Press:

Shift + Enter

to create a new line without sending the message.

---

✍️ Message Display

User and AI messages are displayed as separate chat bubbles.

The application uses:

textContent

for message text instead of directly inserting the user's message as HTML.

---

⏳ Typing Indicator

While waiting for the AI response, the interface displays a typing/loading indicator.

The indicator is removed after the API response is received.

---

🎨 Interface

The application contains:

- Glass-style panels
- Rounded elements
- Animated interface elements
- Chat bubbles
- Provider selector
- Model selector
- API key modal
- Message input
- Send button
- Clear-chat control
- Responsive layout

The main content is limited to a maximum width of approximately:

720px

---

📱 Responsive Design

The CSS includes responsive behavior for smaller screen sizes.

The interface is designed to work on:

Desktop
Tablet
Mobile

---

♿ Reduced Motion

The CSS includes support for users who prefer reduced motion.

The interface can reduce animations when the operating system/browser indicates:

prefers-reduced-motion: reduce

---

🛠️ Technologies Used

This project uses:

HTML

Used for the application structure.

CSS

Used for:

- Layout
- Colors
- Glass effects
- Animations
- Responsive design

JavaScript

Used for:

- Provider selection
- Model selection
- API key handling
- Chat history
- API requests
- API responses
- UI interaction

PHP

PHP is used only as a simple local/server-side web server for serving the HTML project.

The provided application does not contain a PHP backend API.

---

📦 No Database

The provided code does not contain:

MySQL
PostgreSQL
SQLite
Redis
MongoDB

Chat history is stored only in JavaScript memory while the page is open.

---

🚫 No Python Backend

This project does not require:

Python
Flask
FastAPI
Django

A PHP development server can be used to serve the project.

---

🔌 Provider Endpoints

The code contains these API endpoints.

Groq

https://api.groq.com/openai/v1/chat/completions

Google Gemini

https://generativelanguage.googleapis.com/v1beta/models/${model}:generateContent?key=${apiKey}

OpenAI

https://api.openai.com/v1/chat/completions

OpenRouter

https://openrouter.ai/api/v1/chat/completions

Together AI

https://api.together.xyz/v1/chat/completions

Mistral AI

https://api.mistral.ai/v1/chat/completions

Cohere

https://api.cohere.com/v2/chat

---

🧱 Main JavaScript Components

The code contains the following main concepts.

Provider Registry

PROVIDERS

Contains the provider configuration.

---

Provider Order

PROVIDER_ORDER

Controls the provider selection order.

---

API Key

apiKey

Stores the currently entered API key in memory.

---

Provider ID

providerId

Stores the currently selected provider.

---

Model

model

Stores the currently selected model.

---

History

history

Stores the current conversation messages.

---

🔐 API Key Handling

The application sends the API key from the browser to the selected provider.

Therefore, this project is a client-side AI chat interface.

It does not contain a server-side API-key protection layer.

For this reason, API keys should be handled carefully when using the project.

---

📄 Single-File Application

The main advantage of the project structure is that the application can be contained in one HTML file.

index.html

The file contains the:

HTML
CSS
JavaScript

required for the interface.

---

🔧 Basic Setup

1. Create a project folder.

Correspond/

2. Put the HTML file inside it:

Correspond/
└── index.html

3. Open a terminal in that directory.

4. Start PHP:

php -S localhost:8000

5. Open:

http://localhost:8000

6. Select a provider.

7. Enter the provider API key.

8. Select the available model.

9. Enter your message.

10. Send the message.

---

📜 License

No specific license is included in the provided code.

Add a license file separately if you decide to publish the project under a specific open-source license.

---

⚠️ Project Limitations

The provided code does not include:

- User accounts
- Login
- Registration
- PHP API backend
- Database
- Persistent chat storage
- Redis
- File uploads
- Image generation
- Voice chat
- Authentication system
- OTP
- Payment system
- Server-side API-key storage
- Python backend

---

📌 Summary

Correspond is a browser-based multi-provider AI chat interface.

HTML
 ├── Interface
 │
CSS
 ├── Design
 ├── Responsive layout
 └── Animations
 │
JavaScript
 ├── Provider selection
 ├── Model selection
 ├── API key
 ├── Chat history
 ├── API requests
 └── AI responses
 │
PHP Server
 └── Serves the web application

The application communicates directly with the selected AI provider through browser "fetch()" requests.

No database or Python backend is required by the provided code.
