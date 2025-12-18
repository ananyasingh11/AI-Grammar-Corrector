# AI Grammar & Spelling Corrector

A web-based tool effectively leveraging Google's Gemini API to correct grammar and spelling errors in your text. This application offers a clean interface for users to verify and fix their text while preserving original formatting such as line breaks.

## Features

- **Grammar & Spelling Correction**: Uses advanced AI (Google Gemini 1.5 Flash) to identify and fix errors.
- **Format Preservation**: Explicitly handles and maintains the user's original line breaks and spacing.
- **Web Interface**: Simple and responsive UI built with EJS and Express.
- **Error Handling**: specialized error messages for empty inputs or API issues.

## Prerequisites

Before you begin, ensure you have met the following requirements:

- **Node.js**: installed on your local machine (v14 or newer recommended).
- **Gemini API Key**: You need an API key from Google AI Studio. Get one [here](https://aistudio.google.com/app/apikey).

## Installation

1.  **Clone the repository** (if applicable) or navigate to the project folder.

2.  **Install Dependencies**:
    Run the following command to install the required Node.js packages:
    ```bash
    npm install
    ```

## Configuration

1.  Create a `.env` file in the root directory of the project.
2.  Add your Google Gemini API Key and (optinal) Port number:

    ```env
    GEMINI_API_KEY=your_actual_api_key_here
    PORT=5000
    ```

## Usage

1.  **Start the Server**:
    ```bash
    npm start
    ```
    or
    ```bash
    node index.js
    ```

2.  **Open the Application**:
    Visit `http://localhost:5000` in your web browser.

3.  **Correct Text**:
    - Enter your text in the text area.
    - Click the "Correct" button.
    - View the corrected version below the input area.

## Project Structure

```
.
├── index.js        # Main application entry point (Express server)
├── package.json    # Project dependencies and scripts
├── .env            # Environment variables (API keys)
├── views/
│   └── index.ejs   # Frontend template
└── public/         # Static assets (css, images, etc.)
```

## Technologies Used

- **Runtime**: Node.js
- **Framework**: Express.js
- **Templating**: EJS
- **AI Model**: Google Gemini 1.5 Flash (via REST API)
