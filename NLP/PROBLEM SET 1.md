## 1. What is Natural Language Processing (NLP) and why is it important?

Natural Language Processing (NLP) is a subfield of Artificial Intelligence (AI) and Computer Science that focuses on enabling machines to understand, interpret, generate, and interact with human language in a meaningful way.

NLP is essential because it bridges the gap between human communication and computer understanding. It involves collecting textual data, preprocessing it (such as cleaning, tokenization, etc.), and then feeding it into machine learning models to identify patterns and make predictions or decisions based on language input.

NLP has become a cornerstone of modern applications across various domains, including:

1. **Sentiment Analysis** – determining the emotional tone behind reviews, social media posts, or customer feedback.
2. **Spam Detection** – classifying emails or messages as spam or not.
3. **Text Autocompletion and Suggestion** – used in mobile keyboards, search engines, and IDEs.
4. **Conversational Agents and Chatbots** – powering customer service and personal assistants.
5. **Generative AI and Large Language Models (LLMs)** – enabling content creation, summarization, translation, and more.
The growing ubiquity of language-based systems makes NLP a vital tool in both industry and research.

## 2. What do you understand by the terms 'Corpus', 'Tokenization' and 'Stop words' in NLP.

**1. Corpus** –  
In NLP, a _corpus_ refers to a large and structured set of texts. It is the complete body of textual data (documents, sentences, paragraphs) used for training or analyzing language models. For example, a dataset containing 10,000 movie reviews forms a corpus.

**2. Tokenization** –  
Tokenization is the process of breaking down text into smaller units called _tokens_, such as words, sub-words, or characters. For example, the sentence:  
`"I am studying English"`  
can be tokenized into:  
`["I", "am", "studying", "English"]`  
This is a critical first step in converting text into a machine-readable numerical format.

**3. Stop Words** –  
Stop words are commonly used words (like "the", "is", "in", "and") that often do not carry significant meaning in NLP tasks. These are usually removed during preprocessing to reduce noise and dimensionality, especially in models like Bag-of-Words or TF-IDF.  
However, in tasks like sentiment analysis or question answering, stop words may still be important, so their removal is context-dependent.

## 3. What is Morphology in NLP

**Morphology** is the process of analyzing words by breaking them down into **morphemes** — the smallest meaningful units of language.
For example:  
`"unhappiness"` → `un-` (not) + `happy` + `-ness` (state)
Morphology serves as the **foundation for many NLP preprocessing techniques**, such as **stemming** and **lemmatization**.
### Why is it necessary?
Computers don’t understand the meaning behind words by default. To a machine learning model, words like `run`, `runs`, `ran`, `running`, and `runned` may appear as **entirely different tokens** — even though humans can clearly tell they relate to the same concept.

Morphological analysis helps bridge this gap. By breaking words into morphemes, we can better understand the **root meaning** and **grammatical context**.

For instance:  
`"unbreakable"` → `un-` (not) + `break` + `-able` (capable of) → _"not capable of being broken"_

## 4. What is Syntax in NLP

**Syntax** is the study of how words combine to form **valid phrases, clauses, and sentences** — i.e., how the structure of a sentence is built according to **grammar rules**.
#### **Part-of-Speech Tagging (POS Tagging)**
Assigns tags like `noun`, `verb`, `adjective`, etc. to words.
- Helps disambiguate meaning:
    - `book` (noun) vs `book` (verb)
####  2. **Syntactic Parsing (Constituency & Dependency Parsing)**
- Breaks down sentence structure like a **syntax tree**.
- Identifies how words **depend on** or **modify** each other

## 5. Explain POS (Parts of Speech) tagging in NLP

**Part-of-Speech (POS) tagging** is the process of **assigning a part of speech** to each word in a sentence based on its **definition and context**.
`Sentence: The cat sat on the mat.
`POS tags: DET  NOUN VERB PREP DET NOUN

It is important to know about the context of word in sentence. For example in sentence `Book a flight -> Book is a verb` and in the sentence `Read a book -> It is not a verb. It's a noun`. Part of speech tagging helps the models/humans understand context about the sentences and make inferences.
