# chat-voice-gpt-project
Simple project. Speech-to-text / Text-to-speech with chat-gpt

This is a Python script that allows the user to ask a question by speaking into a microphone and getting a response from OpenAI's GPT-3 language model. Here's how it works:

The script initializes the text-to-speech engine (using the pyttsx3 library) and sets the API key for OpenAI.

The transcribe_audio_to_text function takes a filename (corresponding to an audio file) and uses the SpeechRecognition library to transcribe the audio to text using Google's speech recognition API.

The generate_response function takes a prompt (the user's question) and uses OpenAI's GPT-3 language model to generate a response. The max_tokens parameter controls the maximum length of the generated response.

The speak_text function takes some text and uses the initialized text-to-speech engine to speak it out loud.

The main function contains the main loop of the script. It listens for the user to say "Genius", indicating that they want to ask a question. If the user says "Genius", the script starts recording their question using the microphone. The recorded audio is transcribed to text using Google's speech recognition API, and the resulting text is used as the prompt for the GPT-3 language model to generate a response. The response is then spoken out loud using the text-to-speech engine.

Overall, this script provides a simple way to interact with OpenAI's GPT-3 language model using voice input and output.
