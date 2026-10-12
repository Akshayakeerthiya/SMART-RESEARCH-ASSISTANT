# SMART-RESEARCH-ASSISTANT

An LLM-powered research assistant that uses FLAN-T5 Large and TinyLlama to summarize technical articles and answer questions based on their content. Developed using Python, PyTorch, Pandas, and Hugging Face Transformers, the project explores transformer-based text generation for faster and more accessible research analysis.

## Project Overview

The **Smart Research Assistant** simplifies the process of understanding lengthy technical articles by applying Large Language Models (LLMs) to summarization and question answering.

The project experiments with two pretrained transformer models, FLAN-T5 Large and TinyLlama 1.1B Chat. It generates concise article summaries and explores question answering by supplying the article text as context to the language model.

The primary goal is to make technical information easier to understand while reducing the effort required to review lengthy content.

## Objectives

- Develop an assistant for summarizing technical and research articles.
- Generate relevant answers to questions about supplied article content.
- Explore different transformer architectures for text generation.
- Apply prompt engineering to guide model outputs.
- Examine model behavior and limitations when processing lengthy text.

## Key Features

- **Article Summarization:** Condenses lengthy technical content into shorter summaries.
- **Context-Based Question Answering:** Generates answers using the article supplied as input.
- **Multiple Transformer Models:** Experiments with FLAN-T5 Large and TinyLlama 1.1B Chat.
- **Prompt-Based Generation:** Uses task-specific instructions to guide summaries and answers.
- **Dataset Processing:** Loads and explores article data using Pandas.
- **Pretrained Model Integration:** Uses the Hugging Face Transformers library to load and run language models.

## Technologies Used

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Language Models | FLAN-T5 Large, TinyLlama 1.1B Chat |
| NLP Framework | Hugging Face Transformers |
| Deep Learning | PyTorch |
| Data Processing | Pandas |
| Model Repository | Hugging Face Hub |
| Development Environment | Google Colab / Jupyter Notebook |
| Planned User Interface | Streamlit |

## Models Used

### 1. FLAN-T5 Large

FLAN-T5 Large is an encoder-decoder transformer designed for text-to-text tasks.

In this project, it is used to generate concise summaries from technical articles. The implementation also explores the impact of input token limits on processing longer documents.

### 2. TinyLlama 1.1B Chat

TinyLlama 1.1B Chat is a compact, decoder-only language model designed for conversational text generation.

Its role in the project includes:

- Producing summaries of article content.
- Answering questions using article text supplied as context.
- Exploring prompt-based generation with a lightweight language model.

## Project Workflow

1. **Library Initialization:** Import the required data-processing and deep-learning libraries.
2. **Dataset Loading:** Read article titles and full text from `Articles.csv`.
3. **Data Exploration:** Inspect the dataset and select articles for experimentation.
4. **Model Loading:** Initialize the pretrained models and their corresponding tokenizers.
5. **Summary Generation:** Apply task-specific prompts to generate article summaries.
6. **Question Answering:** Combine article content and a user question to generate a response.
7. **Output Inspection:** Review generated results and identify limitations related to input length and response quality.

## Dataset Description

The project uses `Articles.csv`, a structured dataset containing article titles and their corresponding text.

| Column | Description |
|---|---|
| `Title` | Title identifying the article's subject |
| `Article` | Full article text used for summarization and question answering |

The notebook loads the dataset from a configured Google Drive path. Update this path to match your own environment before running the notebook.

## Example Applications

- Summarizing technical and research articles.
- Reviewing emerging technologies and AI developments.
- Extracting key information from lengthy documents.
- Answering questions about specific article content.
- Supporting faster review of technical material.

## Limitations

- Input token limits can prevent the models from processing entire long articles.
- Summaries may omit important details or lose context.
- Generated answers may contain incorrect or unsupported information.
- Output quality depends on the input text, prompts, and generation settings.
- Running large pretrained models can require substantial memory and computing resources.

## Future Enhancements

- Build an interactive Streamlit application.
- Support document uploads and user-provided article text.
- Implement chunk-based processing for lengthy documents.
- Include source references to help users verify generated answers.
- Compare model outputs using consistent evaluation criteria.
- Integrate Retrieval-Augmented Generation (RAG) for searching larger document collections.
- Improve error handling and deployment configuration.
- Deploy the application through Hugging Face Spaces.

## Conclusion

The Smart Research Assistant demonstrates the use of pretrained transformer models for article summarization and question answering. By exploring FLAN-T5 Large and TinyLlama, the project provides practical experience with LLM integration, prompt engineering, and text generation for research-oriented applications.

## Disclaimer

This project is intended for educational purposes. Generated summaries and answers may contain inaccuracies and should be checked against the original source material before being used for research or decision-making.
