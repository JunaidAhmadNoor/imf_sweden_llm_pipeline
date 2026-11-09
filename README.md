# IMF Sweden Report – LLM Pipeline

This is my coursework for Data Analysis with AI.

The notebook reads the IMF report for Sweden (IMF Country Report No. 24/70, 2024 Article IV), pulls out the key numbers and risks with Gemini models, checks them with a second "judge" model, and makes a dashboard.


## What it does

1. Reads the PDF and cleans the text
2. Splits it into chunks (400 tokens, 50 overlap)
3. Summarises the report and each section
4. Finds 7 themes, strengths and risks
5. Extracts 6 indicators as JSON (GDP, inflation, policy rate, NPL, unemployment, Tier 1)
6. Answers questions using RAG (FAISS)
7. Checks the outputs with a judge model
8. Makes a 4-chart dashboard

## How to run

1. Download the report PDF from the IMF eLibrary.
2. Open the notebook in Google Colab.
3. Add your Gemini API key as a Colab secret called `GEMINI_API_KEY`.
4. Click Runtime → Run all.
5. Allow Google Drive access and upload the PDF when asked.

Answers are saved, so running it again is quick.

