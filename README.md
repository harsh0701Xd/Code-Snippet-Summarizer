# **Code-Snippet-Summarizer**

**Project Description :** Metadata generation is necessary to understand existing codes and speed up the process of software maintenance. In this project, a sequence-to-sequence translation architecture is implemented so that code snippets can be used to make a summary string.

**Dataset Description :** Dataset is used from the [Code Search Net challenge](https://github.com/github/CodeSearchNet/) github repository which has released around 2 million code and docstring pairs in 6 programming languages — go, python, php, ruby, java, javascript. Data is stored in jsonlines format. Each line in the uncompressed file represents one example (usually a function with an associated comment).

**Solution approach :** The code and docstring pairs will be pre-processed and used in a encoder decoder architecture (based on recurrent neural networks) with attention to generate docstring from code snippets.

*Input: Code*

*Output: Docstring*

**Method :** Text Preprocessing -> Text Tokenisation -> Sequence Padding -> Encoder Decoder -> Attention -> Generation -> Evaluation using ROUGE or BLEU

![image](https://user-images.githubusercontent.com/89227170/178486363-419ffc97-b5d9-47b2-b969-84aca0b9ff95.png)
