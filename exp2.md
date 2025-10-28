# EXP 2
## i) Sentence Segmentation Techniques:
1. **Aim:** Write a program for Sentence Segmentation Techniques.
   
2. **Requirements:**
    * Computer system with an intel core i3/i5 CPU or above, and 4GB of ram or above.
    * Python 3.7 or above
    * nltk library
      
3. **Program:**
```python
import nltk
import re
nltk.download('punkt')

# Sentence Segmentation
text = "Welcome to NLP. This is sentence segmentation."
sentences = nltk.sent_tokenize(text)
print("Sentences:", sentences)
```
4. **Output:**
   
```Sentences: ['Welcome to NLP.', 'This is sentence segmentation.']```

5. **Conclusion:**
   
   Successfully implemented Python program for sentence segmentation.

## ii) Word Segmentation.
1. **Aim:** Write a program for Word Segmentation using Re and nltk.
   
2. **Requirements:**
    * Computer system with an intel core i3/i5 CPU or above, and 4GB of ram or above.
    * Python 3.7 or above
    * nltk library
    * re module
      
3. **Program:**
```python
import nltk
import re
nltk.download('punkt')

text = "Welcome to NLP. This is sentence segmentation."

# Word Segmentation using re
words = re.findall(r'\b\w+\b', text)
print("Words using re:", words)

# Word Segmentation using nltk
words_nltk = nltk.word_tokenize(text)
print("Words using nltk:", words_nltk)
```
4. **Output:**
   
```
Words using re: ['Welcome', 'to', 'NLP', 'This', 'is', 'sentence', 'segmentation']
Words using nltk: ['Welcome', 'to', 'NLP', '.', 'This', 'is', 'sentence', 'segmentation', '.']
```
5. **Conclusion:**
   
   Successfully implemented Python program for word segmentation using re and nltk.

### 6. Questions:

Q1. **Split the text into word and sentence segmentation.  
Text: “Hello Good Morning! Today is my NLP practical and I am very tensed"**

Sentence segmentation:  
1. Hello Good Morning!
2. Today is my NLP practical and I am very tensed.

Word segmentation:  
* Sentence 1 → ["Hello", "Good", "Morning", "!"]  
* Sentence 2 → ["Today", "is", "my", "NLP", "practical", "and", "I", "am", "very", "tensed", "."]

**Q2. State the library used for sentence segmentation and how to install that library.**

The library used for sentence tokenization is nltk.  
installation command:  
      pip install nltk
