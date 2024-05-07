This is the document chatbot which uses the Mixtral8x7b LLM to Extract information from the uploaded pdf.

## Huggingface
Model is Deployed using streamlit for Huggingface.

Run the code with command : streamlit run Mindcase_LLM.py (Assuming you have a local gpu)

![Front-End](https://github.com/SAaradhya/QnA_Model/blob/main/Images/Screenshot%202024-05-07%20133505.png)

- Huggingface is able to process the files with less than 32,000 tokens only.
- We reduced the file size by removing some pages.
- The final model works fine with the token < 32000.
- To built the model for more than 32k tokens we opt for Groq with same Mixtral8x7b LLM.

## Groq

Use Google Colab for Groq.

### Steps to follow
- Upload the .env file in the colab environment.
- Upload the pdf file to be processed.
- Can upload all the files in the Groq folder for the smooth conduct.
- To opt for different pdf, change the "/content/blade_runner_2049.pdf" to the required pdf name.


