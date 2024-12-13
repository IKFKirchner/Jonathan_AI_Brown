# Jonathan A.I. Brown: Retrieval-Augmented Generation (RAG) for Islamic Studies

## Note
The notebook was an experiment conducted between November 2023 and March 2024 as part of my dissertation research on "Ibn al-Jawzī's Kitāb al-Mawḍūʿāt and the Forging of a Sunni identity" but was not uploaded here until Dec. 2024. As Large Language Models (LLMs) in general, and ChatGPT specifically, evolve rapidly, this notebook may already be outdated. However, I hope that it may provide a useful look "under the hood" and serve as an example of how to approach this sort of thing. 

## Description
Jonathan A.I. Brown is an AI-powered Jupyter Notebook that answers questions in the style of Jonathan A. C. Brown, professor of Islamic Studies at Georgetown University. It leverages OpenAI's GPT-4 model and Retrieval-Augmented Generation (RAG) to give context-aware responses based on Jonathan Brown's works. Using GPT-4 and RAG, the AI retrieves relevant passages from a specified folder of texts and synthesizes them into coherent responses to user queries.

Notable works include:
- **"Misquoting Muhammad: The Challenge and Choices of Interpreting the Prophet's Legacy"**: A critical analysis of the complexities involved in interpreting Islamic texts.
- **"Hadith: Muhammad's Legacy in the Medieval and Modern World"**: An exploration of the role of Hadith in Islamic law and history.
- **"Islamic Law in an Age of Crisis"**: A detailed examination of the challenges faced by Islamic law in contemporary times.
- **"Islam And Blackness"**: A deep exploration of race and Islam, published in 2022.
- **"Slavery And Islam"**: A comprehensive examination of the role of slavery in Islamic history, published in 2019.
- **"Very Short Introduction to Muhammad"**: An accessible introduction to the Prophet Muhammad, published in 2011.
- **"The Canonization of al-Bukhari and Muslim: The Formation and Function of the Sunni Hadith Canon"**: An in-depth look at the Sunni Hadith canon, published in 2007.
- **"The Rules of Matn Criticism: There Are No Rules"**. *Islamic Law and Society*, 19, 4 (2012).
- **"Even if it’s not True it’s True: Using Unreliable Hadiths in Sunni Islam"**. *Islamic Law and Society*, 18 (2011): Jan-52.
- **"The Canonization of Ibn Majah: Authenticity vs. Utility in the Formation of the Sunni Hadith Canon"**. *Revue des Mondes Musalmans et de la Medeterranee*, 129 (2011): 171-83.
- **"Did the Prophet Say It or Not?: the Literal, Historical and Effective Truth of Hadiths in Sunni Islam"**. *Journal of the American Oriental Society*, 129, 2 (2009): 259-85.
- **"How We Know Early Hadith Critics Did Matn Criticism and Why It’s So Hard to Find"**. *Islamic Law and Society*, 15 (2008): 143-84.
- **"Critical Rigor vs. Juridical Pragmatism: How Legal Theorists and Hadith Scholars Approached the Backgrowth of Isnads"**. *Islamic Law and Society*, 14, 1 (2007): Jan-41.

These works serve as the knowledge base for this AI. However, for copyright reasons, the folder of works used for the knowledge base is not included in this repository.

## Code Description
The code for Jonathan A.I. Brown comprises the following components:
1. **PDF Text Extraction**: Reads and extracts text from all PDF files in a specified folder.
2. **Text Indexing**: Splits the extracted text into manageable chunks and creates a vector-based index using ChromaDB for efficient retrieval.
3. **Context Retrieval**: Retrieves the most relevant chunks of text for a given query using similarity search.
4. **AI Response Generation**: Sends the query and retrieved context to OpenAI's GPT-4 API, which generates a detailed response in the style of Jonathan A. C. Brown. 

## Installation Guide
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/jonathan-ai-brown.git
   cd jonathan-ai-brown
   ```
2. Install the required dependencies:
   ```bash
   pip install openai PyPDF2 langchain chromadb tiktoken
   ```
3. Obtain an OpenAI API key by signing up at [OpenAI](https://openai.com/). For budgetary reasons, users must provide their own API key.
4. Replace `your_openai_api_key` in the code with your actual OpenAI API key.

## Usage Guide
1. Prepare a folder of PDF files containing Jonathan A. C. Brown's works.
2. Update the `folder_path` variable in the code with the path to your folder.
3. Run the notebook in Jupyter:
   ```bash
   jupyter notebook
   ```
4. Input a query in the specified section of the notebook to receive a response from "Jonathan A.I. Brown."

## References
- Brown, J. A. C. (2007). The Canonization of al-Bukhārī and Muslim: The Formation and Function of the Sunnī Ḥadīth Canon. Leiden: Brill.
- Ibid. (2007). "Critical Rigor vs. Juridical Pragmatism: How Legal Theorists and Ḥadīth Scholars Approached the Backgrowth of Isnāds." Islamic Law and Society, 14(1), 1–41.
- Ibid. (2008). "How We Know Early Ḥadīth Critics Did Matn Criticism and Why It’s So Hard to Find." Islamic Law and Society, 15(2), 143–184.
- Ibid. (2009). Hadith: Muhammad's Legacy in the Medieval and Modern World. Oxford: Oneworld Publications.
- Ibid. (2009). "Did the Prophet Say It or Not? The Literal, Historical, and Effective Truth of Ḥadīths in Early Sunnism." Journal of the American Oriental Society, 129(2), 259–285.
- Ibid. (2011). "Even if It’s Not True, It’s True: Using Unreliable Ḥadīths in Sunni Islam." Islamic Law and Society, 18(1), 1–52.
- Ibid. (2011). "The Canonization of Ibn Mājah: Authenticity vs. Utility in the Formation of the Sunni Ḥadīth Canon." Revue des Mondes Musulmans et de la Méditerranée, 129, 171–183.
- Ibid. (2011). Muhammad: A Very Short Introduction. Oxford: Oxford University Press.
- Ibid. (2012). "The Rules of Matn Criticism: There Are No Rules." Islamic Law and Society, 19(4), 356–396.
- Ibid. (2014). Misquoting Muhammad: The Challenge and Choices of Interpreting the Prophet's Legacy. London: Oneworld Publications.
- Ibid. (2017). Islamic Law and Society: An Introduction. Cambridge: Cambridge University Press.
- Ibid. (2019). Slavery and Islam. London: Oneworld Publications.
- Ibid. (2022). Islam and Blackness. London: Oneworld Publications.

## Additional Notes
- Users are responsible for providing their own knowledge base of texts. For ethical and privacy considerations, the folder of Jonathan A. C. Brown's works is not included in this repository.
- Users also need to use their own APIs for budgetary reasons.

By following these steps, you can adapt the code for your own purposes or scholarly projects. 
Feedback and contributions are welcome!
