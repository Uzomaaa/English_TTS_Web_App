# Project Title:
# Text-to-Speech App in Nigerian Languages – Team English

# Overview

This project is a simple Text-to-Speech (TTS) web application that allows users to type English text and hear it spoken aloud using AI-generated voices from the ElevenLabs API. Our team focused on the English language, which serves as Nigeria’s official language and the most widely used for communication across sectors.
We also tested how well the ElevenLabs API handles other Nigerian languages such as Yoruba, Igbo, and Pidgin English.

# Technologies Used

•	Python

•	Gradio – for building the web interface

•	ElevenLabs API – for realistic speech generation

•	Google Colab – for development and hosting

# How Does ElevenLabs Handle Different Languages?

•	ElevenLabs uses AI-powered multilingual models, primarily:
o	eleven_multilingual_v2 (latest and most capable)

•	It automatically detects the language of your input text.

•	You do not need to specify the language — it figures it out from the sentence.

•	Voice cloning or custom voices can also be trained for multilingual output.

ElevenLabs supports multiple languages through the eleven_multilingual_v2 model. It uses language detection to read text in English, Yoruba, Igbo, or Pidgin without additional configuration. However, pronunciation quality depends on the voice used and how phonetically close the input is to standard English characters.

# Key Features

•	Text input for English and other Nigerian languages

•	Dropdown to select voice

•	In-browser audio playback and download option

•	Clear UI with helpful emojis and headings

•	Hosted online with shareable link for testing and demo

# Language Focus: English

We tested the app primarily using natural English sentences such as:

“Long long ago, in a small house near the forest, there lived a little girl with her mother. Her name was Little Red Riding Hood.”

# Observations:

•	English speech output was clear, natural, and well-paced.

•	The selected voices (Adam, Alexandra, Andy) produced realistic and expressive audio.

•	Punctuation in the text helped structure the rhythm and pauses.

# Additional Language Testing (Yoruba, Igbo, Pidgin)

•	Pidgin had partial success due to its similarity to English.

•	Yoruba and Igbo did not pronounce correctly — tone, accents, were often misread.

•	The ElevenLabs model (eleven_multilingual_v2) attempts detection, but the voices used were not trained on these languages, leading to robotic outputs.

# How We Tested Pronunciation

1.	Entered English and non-English text into the app.
  
2.	Switched voices to observe pronunciation differences.
   
3.	Evaluated output clarity with both native understanding and external review.

# Voice IDs Used

•	Hank (English Male) – 6F5Zhi321D3Oq7v1oNT4

•	Alexandra (English Female) – kdmDKE6EkgrWrrykO9Qt

•	Andy (English Male) – D38z5RcWu1voky8WS1ja

# Demo Video Highlights

•	Typed in English
•	Chose a voice from the dropdown
•	Clicked “Generate Audio”
•	Played and downloaded the result

# Team Reflection

Building the TTS app with ElevenLabs was a great learning experience. We faced challenges using VSCode, especially with loading the API key from the .env file and handling 401 errors due to “unusual activity.” Despite debugging environment variable paths and trying various fixes, the app only worked reliably on Google Colab, so I switched to Colab to complete the project.
I also tested Igbo, Yoruba, and Pidgin, but the ElevenLabs voices struggled with pronunciation and tone. English output worked well, but local Nigerian languages were not fluent.
This project helped me improve my skills in API integration, debugging, error handling, and building user-friendly web apps with Gradio.



