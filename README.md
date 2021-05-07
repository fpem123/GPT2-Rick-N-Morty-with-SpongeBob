# GPT2-Rick-n-Morty-with-SpongeBob

[![Run on Ainize](https://ainize.ai/images/run_on_ainize_button.svg)](https://ainize.web.app/redirect?git_repo=https://github.com/fpem123/GPT2-Rick-N-Morty-with-SpongeBob)

This project generates Rick and Morty with SpongeBob script using GPT-2 model.

Fine tuning data 1: [Kaggle](https://www.kaggle.com/andradaolteanu/rickmorty-scripts)

Fine tuning data 2: [Kaggle](https://www.kaggle.com/mikhailgaerlan/spongebob-squarepants-completed-transcripts)

Model download: [Hugging face](https://huggingface.co/ainize/gpt2-rnm-with-spongebob)

Fine-tuning notebook: [colab](https://colab.research.google.com/drive/1IYSfeqYePWnU9yMJDLAAZRZDKAcXa2ft#scrollTo=KUsyn02WWmf5)

### Model information

    Base model: e-tony/gpt2-rnm
    Epoch: 2
    Train runtime: 790.0612 secs
    Loss: 2.8569

### How to use:
    * First, Choose Rick and Morty or SpongeBob character name.
    * Second, Fill what the character will say in text. This will be base of script.
    * And then, Fill number in length. Text is created as long as "length". I recommend between 100 and 300.
    * If length is so big, generate time will be long.


### Post parameter
    
    name: The Rick and Morty and SpongeBob character name.
    text: The base of script.
    length: The size of generated text.


### Output foramt

    {"0": [[character name, dialog], [character name, dialog], ...]}


### Image reference

[static/IMG_Reference.md](https://github.com/fpem123/GPT2-Rick-N-Morty-with-SpongeBob/blob/master/static/IMG_Reference.md)

## * With CLI *

### Input example

    curl -X POST "https://master-gpt2-rick-n-morty-with-sponge-bob-fpem123.endpoint.ainize.ai/gen" -H "accept: application/json" -H "Content-Type: multipart/form-data" -F "name=Rick" -F "text=Morty! SpongeBob!" -F "length=100"

### Output example

    {
      "0": [
        [
          "Rick",
          " Morty! SpongeBob! You're the guy!"
        ],
        [
          "SpongeBob",
          " Oh, hi, Morty!"
        ],
        [
          "Rick",
          " I need to hear the story for you because here it is."
        ],
        [
          "Morty",
          " [sighs and falls on his bed playing Bubble Bass music, crying] My goodness, I wish I could live in peace for the rest of my life! [laughs] [walks away]"
        ],
        [
          "Rick",
          " Well, that's not all. [SpongeBob and Rick get into bed as they are"
        ]
      ]
    }

## * With swagger *

API page: [Ainize](https://ainize.ai/fpem123/GPT2-Rick-N-Morty-with-SpongeBob?branch=master)

## * With a Demo *

Demo page: [End-point](https://master-gpt2-rick-n-morty-with-sponge-bob-fpem123.endpoint.ainize.ai/)

<br>
<hr>
