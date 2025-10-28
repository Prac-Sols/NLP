# EXP 3
## i) Porter Stemmer:
1. **Aim:** Apply Lemmatization and Stemming using the Porter Stemmer.
   
2. **Requirements:**
    * Computer system with an intel i3/i5 CPU or above, and 4GB of ram or above.
    * Python 3.7 or above
    * nltk library
      
4. **Program:**
```python
import nltk
from nltk.stem import PorterStemmer, WordNetLemmatizer
nltk.download('wordnet')
nltk.download('omw-1.4')

text = ["running", "flies", "easily", "fairly"]
porter = PorterStemmer()
lemmatizer = WordNetLemmatizer()

stems = [porter.stem(word) for word in text]
lemmas = [lemmatizer.lemmatize(word, pos='v') for word in text]
print('original words:', text)
print('stemmed words:', stems)
print('lemmatized words:', lemmas)
```
4. **Output:**
   
```
original words: ['running', 'flies', 'easily', 'fairly']
stemmed words: ['run', 'fli', 'easili', 'fairli']
lemmatized words: ['run', 'fly', 'easily', 'fairly']
```

5. **Conclusion:**
   
   Successfully implemented Python program for lemmatization and stemming using the Porter Stemmer.

## ii) Lancaster Stemmer:
1. **Aim:** Apply Lemmatization and Stemming using the Lancaster Stemmer.
   
2. **Requirements:**
    * Python 3.7 or above
    * nltk library
      
3. **Program:**
```python
import nltk
from nltk.stem import LancasterStemmer, WordNetLemmatizer
nltk.download('wordnet')
nltk.download('omw-1.4')

text = ["running", "flies", "easily", "fairly"]
lancaster = LancasterStemmer()
lemmatizer = WordNetLemmatizer()

stems = [lancaster.stem(word) for word in text]
lemmas = [lemmatizer.lemmatize(word, pos='v') for word in text]
print('original words:', text)
print('stemmed words:', stems)
print('lemmatized words:', lemmas)
```
4. **Output:**
   
```
original words: ['running', 'flies', 'easily', 'fairly']
stemmed words: ['run', 'fli', 'easy', 'fair']
lemmatized words: ['run', 'fly', 'easily', 'fairly']
```

5. **Conclusion:**
   
   Successfully implemented Python program for lemmatization and stemming using the Lancaster Stemmer.

## iii) Snowball Stemmer:
1. **Aim:** Apply lemmatization and stemming using the Snowball Stemmer.
   
2. **Requirements:**
    * Python 3.7 or above
    * nltk library
      
3. **Program:**
```python
import nltk
from nltk.stem import SnowballStemmer, WordNetLemmatizer
nltk.download('wordnet')
nltk.download('omw-1.4')

text = ["running", "flies", "easily", "fairly"]
snowball = SnowballStemmer(language='english')
lemmatizer = WordNetLemmatizer()

stems = [snowball.stem(word) for word in text]
lemmas = [lemmatizer.lemmatize(word, pos='v') for word in text]
print('original words:', text)
print('stemmed words:', stems)
print('lemmatized words:', lemmas)
```

4. **Output:**
   
```
original words: ['running', 'flies', 'easily', 'fairly']
stemmed words: ['run', 'fli', 'easili', 'fair']
lemmatized words: ['run', 'fly', 'easily', 'fairly']
```

5. **Conclusion:**
   
   Successfully implemented Python program for lemmatization and stemming using the Snowball Stemmer.

### 6. Questions

1. **What is the main difference between stemming and lemmatization in text processing?**
   
* Stemming: Reduces words to their root/stem by chopping off suffixes or prefixes, may not produce a real word.  
* Lemmatization: Reduces words to their dictionary/base form (lemma) using vocabulary and grammatical rules, always produces a valid word..

2. Name one scenario where using a Porter Stemmer might be preferred over a Lancaster Stemmer.
   
   Porter stemmer might be preferred over Lancaster stemmer in a scenario where you want moderate stemming for text retrieval or search engines, since the Porter stemmer is less aggresive than Lancster.
