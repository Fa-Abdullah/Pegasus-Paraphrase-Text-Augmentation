# Pegasus Paraphrase Generator

A text paraphrasing tool using Google's Pegasus model fine-tuned for paraphrase generation, with a Streamlit web interface.

## Overview

This project leverages the `tuner007/pegasus_paraphrase` model to generate multiple paraphrased versions of input text. It provides both a Jupyter notebook implementation and a Streamlit web application for easy interaction.

## Features

- Generate multiple paraphrased versions of any text
- Adjustable number of return sequences (3, 5, or 10)
- Adjustable beam search parameters (5, 10, or 15 beams)
- Streamlit web interface with image-based controls
- Efficient model caching for faster inference

## Technologies

| Component | Technology |
|-----------|-----------|
| Model | Pegasus (tuner007/pegasus_paraphrase) |
| Framework | Hugging Face Transformers |
| UI | Streamlit |
| Tokenization | PegasusTokenizer |
| Generation | Beam Search with temperature sampling |

## How It Works

User inputs text in the Streamlit interface
Select number of beams and return sequences
Model generates multiple paraphrased versions
Results displayed in the interface

## Parameters

Parameter	Description	Options
num_beams	Number of beams for beam search	5, 10, 15
num_return_sequences	Number of paraphrases to generate	3, 5, 10
max_length	Maximum sequence length	60 (fixed)
temperature	Sampling temperature	1.5 (fixed)
Example Output
Input: "The ultimate test of your knowledge is your capacity to convey it to another."

## Output:

"The test of your knowledge is your ability to convey it."
"The ability to convey your knowledge is the ultimate test of your knowledge."
"The test of your knowledge is your ability to communicate it."
"Your capacity to convey your knowledge is the ultimate test of your knowledge."
"The test of your knowledge is how well you can convey it."

## Author
Fatma Abdullah
