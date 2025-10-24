System Architecture

  This system operates as a two-stage sequential pipeline. Its purpose is to answer an English question based on an English context and return the final answer in   French.

  Stage 1: Extractive Question Answering

    An English question and context are provided to a QA model.

    The model extracts the most relevant answer span from the English context.

    Model: distilbert/distilbert-base-cased-distilled-squad

  Stage 2: Machine Translation

    The extracted English answer string is then fed into a translation model.

    This model translates the English string into French, which is returned as the final output.

    Model: Helsinki-NLP/opus-mt-en-fr

Usage Instructions

  Pass your English question and context as string arguments.

  The function will print the intermediate English answer and return the final French answer.

Example

  Given in the file
