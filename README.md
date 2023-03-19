# Voice-enabled Chatbot with GPT-3.5 and Azure Speech Services

This project is a voice-enabled chatbot that uses GPT-3.5 for generating responses and Azure Speech Services for speech-to-text and text-to-speech capabilities. It can recognize and respond to both English and French languages.

## Prerequisites

1. Python 3.6 or higher
2. OpenAI API key
3. Azure Speech Services API key
4. Azure Text Analytics API key

## Installation

1. Clone this repository.

```bash
git clone https://github.com/your-username/AI-pilot-project.git
cd AI-pilot-project
```


2. Create a virtual environment and activate it.
   ```
   python3 -m venv venv
   source venv/bin/activate  # For Linux/MacOS
   venv\Scripts\activate     # For Windows
   ```

3. Install the required packages.

```
pip install -r requirements.txt
```



## Configuration

1. Create a `.env` file in the project root directory.

   ```
   OPENAI_API_KEY=your_openai_api_key
   AZURE_SPEECH_KEY=your_azure_speech_key
   AZURE_SPEECH_REGION=your_azure_speech_region
   TEXT_ANALYTICS_KEY=your_text_analytics_key
   TEXT_ANALYTICS_ENDPOINT=your_text_analytics_endpoint

   ```
2. Replace the placeholder values with your actual API keys and endpoints.

## Usage

1. Run the `elGPT.py` script.

   ```
   python elGPT.py

   ```
2. Speak into your microphone to interact with the chatbot. It will automatically recognize the language (English or French) and respond accordingly.
3. Press `Ctrl+C` to stop the chatbot.

## Troubleshooting

If you encounter issues related to the OpenAI API, such as connection errors or rate limits, consider implementing retry mechanisms or increasing the delay between requests. Refer to the OpenAI documentation for more details on API rate limits and error handling.
