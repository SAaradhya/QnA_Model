This is the document chatbot which uses the Mixtral8x7b LLM to Extract information from the uploaded pdf.

## Huggingface
Model is Deployed using streamlit for Huggingface.

Run the code with command : streamlit run Mindcase_LLM.py (Assuming you have a local gpu)

![Front-End](https://github.com/SAaradhya/QnA_Model/blob/main/Images/Screenshot%202024-05-07%20133505.png)

- Huggingface is able to process the files with less than 32,000 tokens only.
- We reduced the file size by removing some pages (approx. 80).
- The final model works fine with the token < 32000.
- To built the model for more than 32k tokens we opt for Groq with same Mixtral8x7b LLM.

## Groq

Use Google Colab for Groq.

### Steps to follow
- Upload the .env file in the colab environment.
- Upload the pdf file to be processed.
- Can upload all the files in the Groq folder for the smooth conduct.
- To opt for different pdf, change the "/content/blade_runner_2049.pdf" to the required pdf name.


## Results of HuggingFace
- Explain the theme of the movie?
![Result-1](https://github.com/SAaradhya/QnA_Model/blob/main/Images/Screenshot%202024-05-07%20131858.png)
- What is the roles of Deckard in the Movie?
![Result-2](https://github.com/SAaradhya/QnA_Model/blob/main/Images/Screenshot%202024-05-07%20132000.png)

## Results of Groq
- You : Does the script pass the Bechdel test?

Model : The Bechdel test requires that a work of fiction features at least two women who talk to each other about something other than a man. In the provided document, there are two female characters, Luv and JOI. However, the conversation between them does not involve any substantial interaction; they mostly discuss the male character, Officer Deckard. Therefore, the script does not pass the Bechdel test.

- You : How many male and female characters are in the movie?

Model : Based on the information provided, there are 5 male characters and 4 female characters in the movie. The male characters include Deckard, K, Niander Wallace, Sapper, and the Model. The female characters include Freysa, Luv, JOI, and Mariette.

## Errors in the HuggingFace
![Error](https://github.com/SAaradhya/QnA_Model/blob/main/Images/Screenshot%202024-05-07%20112654.png)

