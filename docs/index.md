# Enalsis
-----

## Table of contents:

1. [Documentation]()
2. [Aim](#aim)
3. [Advantages](#advantages)
4. [Disadvantages & Limitations](#disadvantages--limitations)
5. [Future Improvements](#future-improvements)
6. [Installation Instructions](#installation-instructions)
7. [Important files](#important-files)

-----

## Aim

The aim of the project is to provide a **comprehensive** Python **package** for **natural language processing (NLP)** tasks, facilitating **text analysis** and understanding through a range of functionalities. By offering functions for **entity recognition**, **sentiment analysis**, **syntactic parsing**, **spelling correction**, **readability assessment**, and more, the package aims to empower developers and researchers with efficient tools for **processing** and **analyzing textual data**.
Ultimately, the goal is to simplify the **implementation** of **NLP tasks** within **Python projects**, enabling users to extract **valuable insights** from text data with ease and accuracy.

-----

## Advantages

1. **Versatile Functionality**: The project offers a wide array of text analysis tools covering entity recognition, sentiment analysis, syntactic parsing, and more.
2. **User-Friendly Interface**: With clear documentation and an intuitive API, users can easily integrate and utilize the package in their projects.
3. **Reliable Results**: Leveraging established libraries like spaCy and TextBlob ensures accurate and dependable text analysis outcomes.
4. **Customizable**: Users have the flexibility to adjust parameters and fine-tune algorithms to meet specific project requirements.
5. **Contributing to NLP**: By facilitating advancements in natural language processing research, the project plays a role in driving innovation and progress in the field.

-----

## Disadvantages & Limitations

1. **Continuous Improvement**: Ongoing enhancements are necessary for evolving needs, but resource allocation and prioritization may pose challenges.

2. **Customization Constraints**: Addressing highly specialized requirements may require extra effort or external integration, potentially limiting adaptability.

3. **Integration Challenges**: Integrating with emerging technologies may face obstacles like compatibility issues or resource constraints, slowing down progress.

4. **Community Complexities**: Diverse contributions may introduce complexities like conflicting priorities, requiring effective community management.

5. **Learning Curve**: Users may face challenges with the complexity of NLP concepts or contributing to open-source, emphasizing the need for accessible documentation.

-----

## Future Improvements

Certainly, here are five points on potential future enhancements:

1. **Advanced Machine Learning Models**: Integration of state-of-the-art machine learning models, such as transformer-based architectures like BERT or GPT, to improve the accuracy and performance of text analysis tasks.

2. **Multilingual Support**: Expansion of language support beyond English to include a broader range of languages, catering to diverse linguistic datasets and enabling global applications.

3. **Real-time Processing**: Development of real-time processing capabilities to handle streaming data, facilitating dynamic text analysis tasks in applications like social media monitoring or live chat support.

4. **Interactive Visualization**: Implementation of interactive visualization tools to provide intuitive visual representations of text analysis results, enhancing user understanding and exploration of textual data.

5. **Privacy and Security Features**: Integration of enhanced privacy and security features to ensure compliance with data protection regulations and safeguard sensitive information during text analysis processes.

### Additional features to add

- Perform Hate Speech Analysis and Detection on Text
- Perform Topic Modeling on the text
- Intent Recognition of the text

-----

## Installation Instructions

### Step 1: Install Python
If you haven't already, you need to install Python on your system. You can download Python from the official website: [Python Downloads](https://www.python.org/downloads/).

### Step 2: Install an Integrated Development Environment (IDE)
Choose an IDE to work with Python. Some popular options include:

- [PyCharm](https://www.jetbrains.com/pycharm/)
- [Visual Studio Code (VSCode)](https://code.visualstudio.com/)
- [Spyder](https://www.spyder-ide.org/)
- [Jupyter Notebook](https://jupyter.org/install)

Download and install your preferred IDE on your system.

### Step 3: Install Git (Optional but Recommended)
If you want to clone the project directly from GitHub, you need to install Git. You can download Git from the official website: [Git Downloads](https://git-scm.com/downloads).

### Step 4: Clone Your Project Repository (Optional)
If you prefer to work with the project locally, you can clone the project repository to your machine using Git. Open a terminal or command prompt and navigate to the directory where you want to clone the repository. Then run:

```bash
git clone https://github.com/Tanay-Dwivedi/English-pip-Package.git
```

### Step 5: Navigate to the Project Directory
Open your IDE and navigate to the directory where your project is located.

### Step 6: Install Your Package Dependencies
To install the required dependencies for your package to run, open a terminal or command prompt within your IDE and navigate to the project directory. Then run:

```bash
pip install -r requirements.txt
```

This command will install all the required dependencies listed in the `requirements.txt` file, ensuring your package can function properly.

### Step 7: Use Your Package
You can now use your package in your Python scripts. Import it using:

```python
import enalsis
```

Then, you can call the functions provided by your package as needed.

### Additional Notes:
- Ensure that your package's dependencies are listed in a `requirements.txt` file or clearly documented in your project's README.
- Refer to your package's documentation for detailed usage instructions and examples.
- Provide a link to your package's GitHub repository or any other relevant resources for further exploration and support.

-----

## Important files

### Contributing File
- **You can contribute**: We welcome contributions to enhance our project. Check out our [Contributing Guidelines](https://github.com/Tanay-Dwivedi/English-pip-Package/blob/master/CONTRIBUTING.md) to learn how you can get involved, submit bug fixes, suggest new features, and collaborate with us.

### Code of Conduct File
- **You must adhere**: We maintain a friendly and inclusive environment for all contributors and users. Before participating in our community, please review our [Code of Conduct](https://github.com/Tanay-Dwivedi/English-pip-Package/blob/master/CODE_OF_CONDUCT.md) to understand the behavior we expect and the consequences of unacceptable conduct.

### Bug Report File
- **You can report**: Encountered a bug? Let us know! Follow our [Bug Reporting Guidelines](https://github.com/Tanay-Dwivedi/English-pip-Package/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) to provide detailed information about the issue, including steps to reproduce it. Your reports help us improve the project for everyone.

### Request Feature File
- **You can request**: Have an idea for a new feature or enhancement? Share it with us! Check out our [Feature Request Guidelines](https://github.com/Tanay-Dwivedi/English-pip-Package/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) to learn how you can request new features and provide valuable insights into how the project can better meet your needs.

### Changelog File
- **You can track**: Stay up-to-date with our project's changes and improvements. Our [Changelog](https://github.com/Tanay-Dwivedi/English-pip-Package/blob/master/CHANGELOG.md) documents each version's release notes, highlighting new features, bug fixes, and other modifications. It's your guide to what's new and improved.

-----

## **List of functions**


### 1. get_entities()


#### Description:
This function extracts entities from the given text using spaCy's named entity recognition (NER) model. It identifies entities such as persons, organizations, locations, and more.

#### Parameters:
- `text` (str): The input text from which entities are to be extracted.

#### Return Value:
- `entities` (list of tuples): A list of tuples where each tuple contains the text of the entity and its corresponding label.

#### Usage Example:
```python
import enalsis

# Example usage of the function
text = "Apple Inc. is located in Cupertino, California."
entities = enalsis.get_entities(text)
print(entities)
```

#### How to Use
To utilize the `get_entities` function in your Python scripts with the "enalsis" package:

1. Make sure you have installed the required dependencies, including spaCy and its English language model (`en_core_web_sm`).

2. Import the `enalsis` module in your Python script.

3. Call the `get_entities` function, passing the input text as an argument.

4. Retrieve the list of entities returned by the function and use them as needed in your application.

Ensure that the input text is in English, as the function relies on spaCy's English language model for entity recognition. Additionally, consider preprocessing the text if necessary to improve entity extraction accuracy.

-----

### 2. get_sentences()


#### Description:
This function extracts sentences from the given text using spaCy's sentence tokenization. It breaks the text into individual sentences based on punctuation and other linguistic cues.

#### Parameters:
- `text` (str): The input text from which sentences are to be extracted.

#### Return Value:
- `sentences` (list of str): A list of sentences extracted from the input text.

#### Usage Example:
```python
import enalsis

# Example usage of the function
text = "This is a sample text. It contains multiple sentences. Each sentence ends with a period."
sentences = enalsis.get_sentences(text)
print(sentences)
```

#### How to Use
To utilize the `get_sentences` function in your Python scripts with the "enalsis" package:

1. Ensure that you have installed spaCy and its English language model (`en_core_web_sm`).

2. Import the `enalsis` module into your Python script.

3. Call the `get_sentences` function, passing the input text as an argument.

4. Retrieve the list of sentences returned by the function and use them as needed in your application.

Ensure that the input text is in English for accurate sentence extraction. Additionally, consider handling any specific punctuation or formatting requirements in your text preprocessing, if necessary.

-----

### 3. get_adjectives()


#### Description:
This function extracts adjectives from the given text using spaCy's part-of-speech tagging. It identifies words that function as adjectives in the text.

#### Parameters:
- `text` (str): The input text from which adjectives are to be extracted.

#### Return Value:
- `adjectives` (list of str): A list of adjectives extracted from the input text.

#### Usage Example:
```python
import enalsis

# Example usage of the function
text = "The big brown dog chased the small cat."
adjectives = enalsis.get_adjectives(text)
print(adjectives)
```

#### How to Use
To utilize the `get_adjectives` function in your Python scripts with the "enalsis" package:

1. Ensure that you have installed spaCy and its English language model (`en_core_web_sm`).

2. Import the `enalsis` module into your Python script.

3. Call the `get_adjectives` function, passing the input text as an argument.

4. Retrieve the list of adjectives returned by the function and use them as needed in your application.

Ensure that the input text is in English for accurate adjective extraction. Additionally, consider preprocessing the text if necessary to improve extraction accuracy.

-----

### 4. get_adverbs()


#### Description:
This function extracts adverbs from the given text using spaCy's part-of-speech tagging. It identifies words that function as adverbs in the text.

#### Parameters:
- `text` (str): The input text from which adverbs are to be extracted.

#### Return Value:
- `adverbs` (list of str): A list of adverbs extracted from the input text.

#### Usage Example:
```python
import enalsis

# Example usage of the function
text = "He quickly ran to the store."
adverbs = enalsis.get_adverbs(text)
print(adverbs)
```

#### How to Use
To utilize the `get_adverbs` function in your Python scripts with the "enalsis" package:

1. Ensure that you have installed spaCy and its English language model (`en_core_web_sm`).

2. Import the `enalsis` module into your Python script.

3. Call the `get_adverbs` function, passing the input text as an argument.

4. Retrieve the list of adverbs returned by the function and use them as needed in your application.

Ensure that the input text is in English for accurate adverb extraction. Additionally, consider preprocessing the text if necessary to improve extraction accuracy.

-----

### 5. get_nouns()


#### Description:
This function extracts nouns from the given text using spaCy's part-of-speech tagging. It identifies words that function as nouns in the text.

#### Parameters:
- `text` (str): The input text from which nouns are to be extracted.

#### Return Value:
- `nouns` (list of str): A list of nouns extracted from the input text.

#### Usage Example:
```python
import enalsis

# Example usage of the function
text = "The cat sat on the mat."
nouns = enalsis.get_nouns(text)
print(nouns)
```

#### How to Use
To utilize the `get_nouns` function in your Python scripts with the "enalsis" package:

1. Ensure that you have installed spaCy and its English language model (`en_core_web_sm`).

2. Import the `enalsis` module into your Python script.

3. Call the `get_nouns` function, passing the input text as an argument.

4. Retrieve the list of nouns returned by the function and use them as needed in your application.

Ensure that the input text is in English for accurate noun extraction. Additionally, consider preprocessing the text if necessary to improve extraction accuracy.

-----

### 6. get_pronouns()


#### Description:
This function extracts pronouns from the given text using spaCy's part-of-speech tagging. It identifies words that function as pronouns in the text.

#### Parameters:
- `text` (str): The input text from which pronouns are to be extracted.

#### Return Value:
- `pronouns` (list of str): A list of pronouns extracted from the input text.

#### Usage Example:
```python
import enalsis

# Example usage of the function
text = "He went to the park with his friends."
pronouns = enalsis.get_pronouns(text)
print(pronouns)
```

#### How to Use
To utilize the `get_pronouns` function in your Python scripts with the "enalsis" package:

1. Ensure that you have installed spaCy and its English language model (`en_core_web_sm`).

2. Import the `enalsis` module into your Python script.

3. Call the `get_pronouns` function, passing the input text as an argument.

4. Retrieve the list of pronouns returned by the function and use them as needed in your application.

Ensure that the input text is in English for accurate pronoun extraction. Additionally, consider preprocessing the text if necessary to improve extraction accuracy.

-----

### 7. get_proper_nouns()


#### Description:
This function extracts proper nouns from the given text using spaCy's part-of-speech tagging. It identifies words that function as proper nouns in the text.

#### Parameters:
- `text` (str): The input text from which proper nouns are to be extracted.

#### Return Value:
- `proper_nouns` (list of str): A list of proper nouns extracted from the input text.

#### Usage Example:
```python
import enalsis

# Example usage of the function
text = "John visited New York last summer."
proper_nouns = enalsis.get_proper_nouns(text)
print(proper_nouns)
```

#### How to Use
To utilize the `get_proper_nouns` function in your Python scripts with the "enalsis" package:

1. Ensure that you have installed spaCy and its English language model (`en_core_web_sm`).

2. Import the `enalsis` module into your Python script.

3. Call the `get_proper_nouns` function, passing the input text as an argument.

4. Retrieve the list of proper nouns returned by the function and use them as needed in your application.

Ensure that the input text is in English for accurate proper noun extraction. Additionally, consider preprocessing the text if necessary to improve extraction accuracy.

-----

### 8. get_verbs()


#### Description:
This function extracts verbs from the given text using spaCy's part-of-speech tagging. It identifies words that function as verbs in the text.

#### Parameters:
- `text` (str): The input text from which verbs are to be extracted.

#### Return Value:
- `verbs` (list of str): A list of verbs extracted from the input text.

#### Usage Example:
```python
import enalsis

# Example usage of the function
text = "She runs every morning."
verbs = enalsis.get_verbs(text)
print(verbs)
```

#### How to Use
To utilize the `get_verbs` function in your Python scripts with the "enalsis" package:

1. Ensure that you have installed spaCy and its English language model (`en_core_web_sm`).

2. Import the `enalsis` module into your Python script.

3. Call the `get_verbs` function, passing the input text as an argument.

4. Retrieve the list of verbs returned by the function and use them as needed in your application.

Ensure that the input text is in English for accurate verb extraction. Additionally, consider preprocessing the text if necessary to improve extraction accuracy.

-----

### 9. get_numbers()


#### Description:
This function extracts numbers from the given text using spaCy's part-of-speech tagging. It identifies words that represent numerical values in the text.

#### Parameters:
- `text` (str): The input text from which numbers are to be extracted.

#### Return Value:
- `numbers` (list of str): A list of numbers extracted from the input text.

#### Usage Example:
```python
import enalsis

# Example usage of the function
text = "There are 10 apples in the basket."
numbers = enalsis.get_numbers(text)
print(numbers)
```

#### How to Use
To utilize the `get_numbers` function in your Python scripts with the "enalsis" package:

1. Ensure that you have installed spaCy and its English language model (`en_core_web_sm`).

2. Import the `enalsis` module into your Python script.

3. Call the `get_numbers` function, passing the input text as an argument.

4. Retrieve the list of numbers returned by the function and use them as needed in your application.

Ensure that the input text is in English for accurate number extraction. Additionally, consider preprocessing the text if necessary to improve extraction accuracy.

-----

### 10. detect_language()


#### Description:
This function detects the language of the given text using the langid library. It analyzes the text and identifies the language it is written in.

#### Parameters:
- `text` (str): The input text whose language is to be detected.

#### Return Value:
- `language_name` (str): The name of the language detected in the input text.

#### Usage Example:
```python
import enalsis

# Example usage of the function
text = "Bonjour tout le monde!"
language = enalsis.detect_language(text)
print(language)
```

#### How to Use
To utilize the `detect_language` function in your Python scripts with the "enalsis" package:

1. Ensure that you have installed the "langid" library, which is a dependency of the "enalsis" package.

2. Import the `enalsis` module into your Python script.

3. Call the `detect_language` function, passing the input text as an argument.

4. Retrieve the detected language name returned by the function and use it as needed in your application.

Keep in mind that the accuracy of language detection may vary depending on the input text and the language models used by the library.

-----

### 11. parse_syntax_tree()


#### Description:
This function performs syntax tree analysis on the given text using spaCy's dependency parsing capabilities. It constructs a syntax tree for the text, providing information about the syntactic structure of the sentences.

#### Parameters:
- `text` (str): The input text for which syntax tree analysis is to be performed.

#### Return Value:
- `syntax_tree_dict` (list of dicts): A list of dictionaries where each dictionary represents a token in the text and contains information such as the token's text, dependency relation, part-of-speech tag, and its head token.

#### Usage Example:
```python
import enalsis

# Example usage of the function
text = "The cat sat on the mat."
syntax_tree = enalsis.parse_syntax_tree(text)
print(syntax_tree)
```

#### How to Use
To utilize the `parse_syntax_tree` function in your Python scripts with the "enalsis" package:

1. Ensure that you have installed spaCy and its English language model (`en_core_web_sm`).

2. Import the `enalsis` module into your Python script.

3. Call the `parse_syntax_tree` function, passing the input text as an argument.

4. Retrieve the syntax tree dictionary returned by the function and use it as needed in your application.

This function provides valuable insights into the syntactic structure of the text, which can be utilized for tasks such as parsing, grammar checking, and syntactic analysis.

-----

### 12. get_POS_tag()


#### Description:
This function extracts part-of-speech (POS) tags from the given text using spaCy's POS tagging capabilities. It assigns a grammatical category to each token in the text, such as noun, verb, adjective, etc.

#### Parameters:
- `text` (str): The input text from which POS tags are to be extracted.

#### Return Value:
- `pos_list` (list of dicts): A list of dictionaries where each dictionary contains information about a token's word and its corresponding POS tag.

#### Usage Example:
```python
import enalsis

# Example usage of the function
text = "The cat sat on the mat."
pos_tags = enalsis.get_POS_tag(text)
print(pos_tags)
```

#### How to Use
To utilize the `get_POS_tag` function in your Python scripts with the "enalsis" package:

1. Make sure you have installed spaCy and its English language model (`en_core_web_sm`).

2. Import the `enalsis` module into your Python script.

3. Call the `get_POS_tag` function, passing the input text as an argument.

4. Retrieve the list of POS tags returned by the function and use them as needed in your application.

Understanding the POS tags of the text can be helpful for various natural language processing tasks such as text classification, information extraction, and sentiment analysis.

-----

### 13. spell_check_text()


#### Description:
This function performs spell-checking on the given text using the TextBlob library. It identifies misspelled words in the text and provides the corrected version of the text.

#### Parameters:
- `text` (str): The input text to be spell-checked.

#### Return Value:
- `misspelled_words` (list): A list of misspelled words found in the input text.
- `corrected_text` (str): The corrected version of the input text with misspelled words replaced.

#### Usage Example:
```python
import enalsis

# Example usage of the function
text = "Thiss is a misspeled sentence."
misspelled_words, corrected_text = enalsis.spell_check_text(text)
print("Misspelled Words:", misspelled_words)
print("Corrected Text:", corrected_text)
```

#### How to Use
To utilize the `spell_check_text` function in your Python scripts with the "enalsis" package:

1. Ensure you have installed the TextBlob library.

2. Import the `enalsis` module into your Python script.

3. Call the `spell_check_text` function, passing the input text as an argument.

4. Retrieve the list of misspelled words and the corrected text returned by the function.

5. Use the corrected text for further analysis or processing in your application.

Spell-checking can help improve the accuracy and readability of text data, particularly in applications where precise language is required, such as document analysis, sentiment analysis, or machine translation.

-----

### 14. find_spell_corrections()


#### Description:
This function identifies misspelled words in the given text and provides their respective corrected versions using the TextBlob library.

#### Parameters:
- `text` (str): The input text in which misspelled words are to be identified and corrected.

#### Return Value:
- `misspelled_dict` (dict): A dictionary where keys represent misspelled words and values represent their respective corrected versions.

#### Usage Example:
```python
import enalsis

# Example usage of the function
text = "Thiss is a misspeled sentence."
misspelled_dict = enalsis.find_spell_corrections(text)
print("Misspelled Word Corrections:", misspelled_dict)
```

#### How to Use
To utilize the `find_spell_corrections` function in your Python scripts with the "enalsis" package:

1. Ensure you have installed the TextBlob library.

2. Import the `enalsis` module into your Python script.

3. Call the `find_spell_corrections` function, passing the input text as an argument.

4. Retrieve the dictionary containing misspelled words and their respective corrected versions returned by the function.

5. Use the corrected text for further analysis or processing in your application.

Spell-checking can help improve the accuracy and readability of text data, particularly in applications where precise language is required, such as document analysis, sentiment analysis, or machine translation.

-----

### 15. profanity_analysis()


#### Description:
This function analyzes the input text for profanity and obscene language using a pre-trained model. It calculates a profanity score and probability indicating the likelihood of the text containing offensive language.

#### Parameters:
- `text` (str): The input text to be analyzed for profanity.

#### Return Value:
- `is_profane` (bool): A boolean value indicating whether the text is considered profane (True) or not (False).
- `profanity_score` (float): A numerical score representing the degree of profanity detected in the text.
- `profanity_prob` (float): The probability of the text containing offensive language, ranging from 0 to 1.

#### Usage Example:
```python
import enalsis

# Example usage of the function
text = "This is a clean text."
is_profane, profanity_score, profanity_prob = enalsis.profanity_analysis(text)
print("Is Profane:", is_profane)
print("Profanity Score:", profanity_score)
print("Profanity Probability:", profanity_prob)
```

#### How to Use:
To utilize the `profanity_analysis` function in your Python scripts with the "enalsis" package:

1. Ensure you have installed the required dependencies, including the pre-trained profanity detection model.
2. Import the `enalsis` module into your Python script.
3. Call the `profanity_analysis` function, passing the input text as an argument.
4. Receive the profanity analysis results, including whether the text is profane, the profanity score, and the probability of profanity.
5. Use the results to filter or flag potentially offensive content in your application.

Profanity analysis can be useful in content moderation, sentiment analysis, and filtering inappropriate text in online platforms or communication channels.

-----

### 16. sentiment_analysis()


#### Description:
This function performs sentiment analysis on the input text using the TextBlob library. It calculates the sentiment polarity of the text, indicating whether it is positive, negative, or neutral. Additionally, it identifies the most frequent sentiment-associated words in the text.

#### Parameters:
- `text` (str): The input text to be analyzed for sentiment.

#### Return Value:
- `results` (dict): A dictionary containing the sentiment analysis results, including:
  - `sentiment_label` (str): The sentiment label indicating whether the text is positive, negative, or neutral.
  - `sentiment_polarity` (float): The sentiment polarity score of the text, ranging from -1 (most negative) to 1 (most positive).
  - `sentiment_words` (list of dicts): A list of dictionaries, each containing:
    - `word` (str): The sentiment-associated word.
    - `score` (float): The sentiment polarity score of the word.
    - `frequency` (int): The frequency of occurrence of the word in the text.

#### Usage Example:
```python
import enalsis

# Example usage of the function
text = "This is a very positive sentence."
results = enalsis.sentiment_analysis(text)
print("Sentiment Label:", results['sentiment_label'])
print("Sentiment Polarity:", results['sentiment_polarity'])
print("Sentiment Words:", results['sentiment_words'])
```

#### How to Use:
To utilize the `sentiment_analysis` function in your Python scripts with the "enalsis" package:

1. Ensure you have installed the TextBlob library.
2. Import the `enalsis` module into your Python script.
3. Call the `sentiment_analysis` function, passing the input text as an argument.
4. Receive the sentiment analysis results, including the sentiment label, sentiment polarity, and sentiment-associated words.
5. Utilize the results to gain insights into the sentiment of the text and analyze sentiment trends in your data.

-----

### 17. semantic_similarity()


#### Description:
This function calculates the semantic similarity between two input texts using the spaCy library. It computes the similarity score based on the cosine similarity between the vector representations of the texts obtained from the pre-trained word vectors in the spaCy medium-sized English language model.

#### Parameters:
- `text1` (str): The first input text for semantic similarity comparison.
- `text2` (str): The second input text for semantic similarity comparison.

#### Return Value:
- `similarity_score` (float): The semantic similarity score between the two input texts, ranging from 0 (least similar) to 1 (most similar).

#### Usage Example:
```python
import enalsis

# Example usage of the function
text1 = "I enjoy reading books."
text2 = "Reading is one of my favorite hobbies."
similarity_score = enalsis.semantic_similarity(text1, text2)
print("Semantic Similarity Score:", similarity_score)
```

#### How to Use:
To utilize the `semantic_similarity` function in your Python scripts with the "enalsis" package:

1. Ensure you have installed the spaCy library with the medium-sized English language model (`en_core_web_md`).
2. Import the `enalsis` module into your Python script.
3. Call the `semantic_similarity` function, passing the two input texts as arguments.
4. Receive the semantic similarity score, indicating the degree of similarity between the two texts.
5. Utilize the similarity score to assess the semantic resemblance between texts, which can be helpful in various NLP tasks such as duplicate detection, recommendation systems, and information retrieval.

-----

### 18. text_summarization()


#### Description:
This function generates a summary of the input text by selecting the most informative sentences. It utilizes a basic approach to extract important sentences based on the frequency of occurrence of words within those sentences. Stop words are removed from consideration to focus on meaningful content.

#### Parameters:
- `text` (str): The input text for which a summary is to be generated.
- `num_lines` (int): The desired number of sentences in the summary.

#### Return Value:
- `summary` (str): A summarized version of the input text containing the most relevant sentences based on word frequency.

#### Usage Example:
```python
import enalsis

# Example usage of the function
text = "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat."
num_lines = 2
summary = enalsis.text_summarization(text, num_lines)
print("Text Summary:", summary)
```

#### How to Use:
To utilize the `text_summarization` function in your Python scripts with the "enalsis" package:

1. Ensure you have installed the NLTK library.
2. Import the `enalsis` module into your Python script.
3. Call the `text_summarization` function, passing the input text and the desired number of sentences in the summary.
4. Receive the summarized version of the input text, which contains the most relevant sentences.
5. Adjust the `num_lines` parameter to control the length of the summary according to your requirements.

-----

### 19. calculate_readability_metrics()


#### Description:
This function calculates various readability metrics for the given text, providing insights into the complexity and ease of comprehension. It computes metrics such as the Flesch Reading Ease, Flesch-Kincaid Grade Level, SMOG Index, Coleman-Liau Index, Automated Readability Index, Dale-Chall Readability Score, and others.

#### Parameters:
- `text` (str): The input text for which readability metrics are to be calculated.

#### Return Value:
- `readability_metrics` (dict): A dictionary containing various readability metrics along with their corresponding values computed for the input text.

#### Usage Example:
```python
import enalsis

# Example usage of the function
text = "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua."
readability_metrics = enalsis.calculate_readability_metrics(text)
print("Readability Metrics:", readability_metrics)
```

#### How to Use:
To utilize the `calculate_readability_metrics` function in your Python scripts with the "enalsis" package:

1. Ensure you have installed the textstat library.
2. Import the `enalsis` module into your Python script.
3. Call the `calculate_readability_metrics` function, passing the input text as an argument.
4. Receive a dictionary containing various readability metrics computed for the input text.
5. Analyze the readability metrics to assess the complexity and ease of comprehension of the text.

-----

### 20. paragraph_sentiment_analysis()


#### Description:
This function performs sentiment analysis on each paragraph of the given text, providing sentiment scores for each paragraph separately. It utilizes the TextBlob library to compute the polarity of each paragraph, indicating whether the sentiment is positive, negative, or neutral.

#### Parameters:
- `text` (str): The input text containing multiple paragraphs for which sentiment analysis is to be performed.

#### Return Value:
- `sentiments` (list): A list containing sentiment scores for each paragraph in the input text. Positive scores indicate positive sentiment, negative scores indicate negative sentiment, and zero indicates neutral sentiment.

#### Usage Example:
```python
import enalsis

# Example usage of the function
text = "Lorem ipsum dolor sit amet, consectetur adipiscing elit.\nSed do eiusmod tempor incididunt ut labore et dolore magna aliqua.\n\nUt enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat."
sentiments = enalsis.paragraph_sentiment_analysis(text)
print("Paragraph Sentiment Scores:", sentiments)
```

#### How to Use:
To utilize the `paragraph_sentiment_analysis` function in your Python scripts with the "enalsis" package:

1. Import the `enalsis` module into your Python script.
2. Call the `paragraph_sentiment_analysis` function, passing the input text containing multiple paragraphs as an argument.
3. Receive a list containing sentiment scores for each paragraph in the input text.
4. Analyze the sentiment scores to understand the overall sentiment distribution across paragraphs and identify any patterns or trends.

-----

### 21. sentence_sentiment_analysis()


#### Description:
This function conducts sentiment analysis on each sentence within the given text, providing sentiment scores for individual sentences. It utilizes the TextBlob library to compute the polarity of each sentence, indicating whether the sentiment is positive, negative, or neutral.

#### Parameters:
- `text` (str): The input text containing multiple sentences for which sentiment analysis is to be performed.

#### Return Value:
- `sentiments` (list): A list containing sentiment scores for each sentence in the input text. Positive scores indicate positive sentiment, negative scores indicate negative sentiment, and zero indicates neutral sentiment.

#### Usage Example:
```python
import enalsis

# Example usage of the function
text = "This is a positive sentence. This is a negative sentence. This sentence is neutral."
sentiments = enalsis.sentence_sentiment_analysis(text)
print("Sentence Sentiment Scores:", sentiments)
```

#### How to Use:
To utilize the `sentence_sentiment_analysis` function in your Python scripts with the "enalsis" package:

1. Import the `enalsis` module into your Python script.
2. Call the `sentence_sentiment_analysis` function, passing the input text containing multiple sentences as an argument.
3. Receive a list containing sentiment scores for each sentence in the input text.
4. Analyze the sentiment scores to understand the sentiment distribution across sentences and identify any patterns or trends.

-----

### 22. extract_word_meanings()


#### Description:
This function extracts words from the given text and retrieves their respective meanings using WordNet, a lexical database for the English language.

#### Parameters:
- `text` (str): The input text from which words and their meanings are to be extracted.

#### Return Value:
- `word_meanings` (list of dicts): A list of dictionaries where each dictionary contains a word and its corresponding meanings retrieved from WordNet.

#### Usage Example:
```python
from your_package import extract_word_meanings

# Example usage of the function
text = "The quick brown fox jumps over the lazy dog."
word_meanings = extract_word_meanings(text)
print("Words and Their Meanings:", word_meanings)
```

#### How to Use:
To utilize the `extract_word_meanings` function in your Python scripts with the package:

1. Ensure you have installed the necessary dependencies, including NLTK and WordNet.

2. Import the `extract_word_meanings` function from your package.

3. Call the `extract_word_meanings` function, passing the input text as an argument.

4. Retrieve the list of dictionaries containing words and their respective meanings returned by the function.

5. Utilize the extracted word meanings for various purposes such as semantic analysis, text understanding, or language processing tasks.

-----

### 23. count_words()


#### Description:
This function extracts words from the given text along with their respective frequencies (i.e., how many times each word appears in the text). It utilizes regular expressions to find all word tokens and then counts their occurrences using the `Counter` class from the `collections` module.

#### Parameters:
- `text` (str): The input text from which words and their frequencies are to be extracted.

#### Return Value:
- List of tuples: Each tuple contains a word and its corresponding frequency in the text.

#### Usage Example:
```python
import enalsis

# Example usage of the function
text = "The quick brown fox jumps over the lazy dog."
word_frequencies = enalsis.count_words(text)
print("Word Frequencies:", word_frequencies)
```

#### How to Use:
To utilize the `count_words` function in your Python scripts with the "enalsis" package:

1. Import the `enalsis` module into your Python script.
2. Call the `count_words` function, passing the input text as an argument.
3. The function will return a list of tuples, where each tuple contains a word and its corresponding frequency in the text.
4. Optionally, you can iterate over the list of tuples to access individual word-frequency pairs for further analysis or processing.

-----

### 24. calculate_alphabetical_and_numberical_percentages()


#### Description:
This function calculates the percentage of alphabetical, numerical, and whitespace characters in the given text. It counts the total number of characters, alphabetical characters, numerical characters, and whitespace characters in the text, and then calculates the respective percentages based on these counts.

#### Parameters:
- `text` (str): The input text from which the percentages are to be calculated.

#### Return Value:
- Tuple: A tuple containing three percentage values representing the proportion of alphabetical characters, numerical characters, and whitespace characters in the text, respectively.

#### Usage Example:
```python
import enalsis

# Example usage of the function
text = "The quick brown fox jumps over the 123 lazy dogs."
alphabetic_percentage, numerical_percentage, whitespace_percentage = enalsis.calculate_alphabetical_and_numberical_percentages(text)
print("Alphabetic Percentage:", alphabetic_percentage)
print("Numerical Percentage:", numerical_percentage)
print("Whitespace Percentage:", whitespace_percentage)
```

#### How to Use:
To utilize the `calculate_alphabetical_and_numberical_percentages` function in your Python scripts with the "enalsis" package:

1. Import the `enalsis` module into your Python script.
2. Call the `calculate_alphabetical_and_numberical_percentages` function, passing the input text as an argument.
3. The function will return a tuple containing three percentage values representing the proportion of alphabetical characters, numerical characters, and whitespace characters in the text.
4. You can then access and utilize these percentage values as needed for further analysis or processing.

----

## Summary

The **enalsis** package offers a comprehensive suite of text analysis tools designed to facilitate various linguistic and semantic tasks. With functions covering a wide range of functionalities, users can easily perform tasks such as entity extraction, sentiment analysis, readability assessment, and more. This Python package leverages popular libraries such as spaCy, NLTK, and TextBlob to provide efficient and accurate analysis capabilities.

-----