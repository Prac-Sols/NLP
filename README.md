# NLP
## EXP 1
Brown Corpus:
1. **Aim:** Implement a program to use Brown corpus OR ii)Penn Treebank Corpus.
   
3. **Requirements:**
    * Python 3.7 or above
    * nltk library
      
4. **Program:**
```python
import nltk
from nltk.corpus import brown

# Download necessary corpus
nltk.download('brown')

words = brown.words(categories='fiction')
print(words[:10])
```
5. **Conclusion:**
   
   Successfully implemented program Python program using the Brown Corpus.
