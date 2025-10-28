
## Exp 4
1. **Aim:** Write program on Text Normalization using nltk & tokenize text & remove special characters.
   
2. **Requirements:**
    * Computer system with an intel i3/i5 CPU or above, and 4GB of ram or above.
    * Python 3.7 or above
    * nltk library
  
3. **Program:**
```python
import nltk
import re
from nltk.tokenize import word_tokenize
nltk.download('punkt')

text = "I'm learning NLP!!! It's fun, isn't it?"

tokens = word_tokenize(text)
clean_text = re.sub(r'[^a-zA-Z\s]', '', text)

print('tokenization result:', tokens)
print('removed special characters:', clean_text)
```

4. **Output:**
```
tokenization result: ['I', "'m", 'learning', 'NLP', '!', '!', '!', 'It', "'s", 'fun', ',', 'is', "n't", 'it', '?']
removed special characters: Im learning NLP Its fun isnt it
```

5. **Conclusion:**
   Successfully implemented python program on test normalization, using nltk to tokenize text and removed special characters.

6. **Questions:**
    1. **What is the purpose of removing special characters from a text during text normalization?**  
        * Clean the text to reduce noise for NLP tasks.
        * Prevent misinterpretation by algorithms.
  
    2. **What is a bigram? Give an example from the sentence: "I love NLP".**  
        * A bigram is a sequence of two consecutive words in a text.  
        * Example from the sentence: "I love NLP": 
          Bigrams:  
          (I, love)  
          (love, NLP)
