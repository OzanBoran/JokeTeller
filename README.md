# Joke Text-to-Speech Generator

This JavaScript application utilizes the VoiceRSS API to convert random jokes from the JokeAPI into speech. The generated audio is played through an HTML audio element, providing an interactive and entertaining experience. This repository serves as a simple project demonstrating the integration of text-to-speech functionality.

## Table of Contents

- [Features](#features)
- [Prerequisites](#Prerequisites)
- [Getting Started](#Getting-Started)
- [JavaScript Methods](#javascript-methods)
- [Deployment](#deployment)

## Features

- Fetches random jokes from the JokeAPI.
- Utilizes the VoiceRSS API for text-to-speech conversion.
- Plays the generated audio through an HTML audio element.
- Disables the button during the API request to prevent multiple requests.

## Prerequisites

- **VoiceRSS API Key:** Obtain a valid API key from [VoiceRSS](https://www.voicerss.org/).

## Getting Started

1. Clone the repository to your local machine:

    ```bash
    git clone https://github.com/OzanBoran/JokeTeller.git
    ```

2. Navigate to the project directory:

    ```bash
    cd JokeTeller
    ```

3. Open the HTML file in a web browser.

4. Click the "Tell me a joke" button to fetch and play a random joke.

### JavaScript Methods:

1. **`document.getElementById('button')`**: Retrieves the button element from the DOM and stores it in the `button` variable.

2. **`document.getElementById('audio')`**: Fetches the audio element from the DOM and assigns it to the `audioElement` variable.

3. **`toggleButton()` Function**: Toggles the `disabled` attribute of the button, enabling or disabling it.

4. **`tellMe(joke)` Function**: Uses the VoiceRSS API to convert a joke into speech, specifying parameters like API key, language, voice, etc.

5. **`getJokes()` Function**: Fetches a random joke from JokeAPI, processes the data, and calls `tellMe` to convert and play the joke using text-to-speech. Disables the button during the API request.

6. **Event Listeners**: Adds click and ended event listeners to the button and audio elements, triggering the respective functions.

## Deployment

The project is deployed and can be accessed online at: https://ozan-boran.github.io/JokeTeller/

## Credits
- **Developer:** Ozan Boran
