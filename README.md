# Voice Recognition Personal Assistant

A voice recognition personal assistant built using Python for office environments. This assistant can execute various commands, such as playing music, fetching data, telling jokes, creating Jira tickets, and more, enhancing productivity through voice commands and task automation.

## Features

- **Play Music:** Search and play songs on YouTube with simple voice commands.
- **Fetch Current Time:** Get the current time by asking.
- **Wikipedia Integration:** Fetch summaries for queries directly from Wikipedia.
- **Tell Jokes:** Lighten the mood with random jokes.
- **Open Websites:** Open specified URLs or predefined websites such as an HR portal.
- **Create Jira Tickets:** Automate the creation of Jira bug tickets with voice commands.
- **Conversational Responses:** Engaging interactions with responses to questions like "Are you single?" or "Tell me a joke."

## Setup

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-repo/voice-assistant.git
   cd voice-assistant
   ```

2. **Install Dependencies:**
   Make sure you have Python 3.x installed. Install the required packages using pip:
   ```bash
   pip install -r requirements.txt
   ```

3. **Configure Jira API:**
   Update the `createJiraTicket` function with your Jira API credentials:
   ```python
   headers = { "Authorization": "Basic <your_encoded_credentials>",
               "Content-Type": "application/json" }
   ```

4. **Run the Assistant:**
   Start the assistant by running the script:
   ```bash
   python assistant.py
   ```

## Usage

1. Activate the microphone and say `Virgil` followed by your command.
2. Examples of supported commands:
   - "Play [song name]"
   - "What time is it?"
   - "Who the heck is [person's name]?"
   - "Tell me a joke."
   - "Create a Jira ticket."

3. For Jira tickets, the assistant will prompt you to enter the summary and description of the bug via the console.

## Dependencies

- `speech_recognition`: For capturing and processing voice input.
- `pyttsx3`: For text-to-speech functionality.
- `pywhatkit`: For YouTube search and playback.
- `wikipedia`: For fetching summaries of topics.
- `pyjokes`: For generating jokes.
- `requests`: For API calls and fetching HTML content.
- `beautifulsoup4`: For parsing HTML data.
- `webbrowser`: For opening URLs in a browser.

## Customization

You can easily extend the functionality by adding new commands in the `run_alexa` function. Each command should have its own `elif` block.

## Future Enhancements

- Add support for additional voice commands.
- Implement natural language understanding for better command recognition.
- Integrate with other productivity tools like Slack or Trello.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

---

Feel free to contribute to this project by submitting issues or pull requests!
