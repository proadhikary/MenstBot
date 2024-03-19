# MenstBot

MenstBot is a menstrual health chatbot based on Llama2, designed to provide information and support regarding menstruation-related queries. This README provides instructions on how to set up and use MenstBot.

## Prerequisites

Before installing and using MenstBot, ensure you have the following:

- Python 3.6 or higher installed on your system.
- Required Python packages:
  - langchain
  - chainlit
  - sentence-transformers
  - faiss
  - PyPDF2 (for loading PDF documents)

## Installation

1. Clone this repository to your local machine:

```bash
git clone https://github.com/proadhikary/MenstBot.git
cd MenstBot
```

2. (Optional but recommended) Create a Python virtual environment:

```bash
python -m venv menstbot
source menstbot/bin/activate
```

3. Install the required Python packages:

```bash
pip install -r requirements.txt
```

## Usage

To use MenstBot, follow these steps:

1. Start the bot by running:

```bash
chainlit app.py -w
```
Which should run at http://localhost:8080/

2. Send a menstruation-related query to the bot.

3. The bot will provide a response based on the information available in its database.

4. If sources are found, they will be provided alongside the answer.

5. Customize the bot to return specific information based on the query and context provided. To do that, add more PDF files in the `data` folder, and run:
```
python ingest.py   
```
6. Enjoy your customized chatbot offline!
