# Anki Automation

This project allows to:
- Add notes
- Add models
- Modify models

It is possible to prompt ChatGPT to generate lists of the items that need to be added, create the models and notes in a format that Anki understands and write in the Anki database using the Anki-Connect API

## Add notes
1. Ask ChatGPT for a python dictionary contaning: 
    * word
    * type of word (noun, verb,adjective)
    * variations (declensions or conjugations)
    * pattern (gender, conjugation group, etc)

2. Generate json object with the note information
3. Send post request to the Anki-Connect API

## Modify Models
This mainly involves to add and modify card templates

## To Do
1. Check if the note already exists
2. Pass a dictionary or json as context for chatGPT
3. Extract the response from chatGPT (word, translation, grammar cases)
4. Create the template for the note
5. Add the note to Anki
6. Add info about OpenAI api-key