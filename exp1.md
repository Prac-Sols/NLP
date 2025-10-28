## EXP 1
### Using the Brown Corpus:
1. **Aim:** Implement a program to use the Brown corpus.
   
2. **Requirements:**
    * Python 3.7 or above
    * nltk library
      
3. **Program:**
```python
import nltk
from nltk.corpus import brown

# Download necessary corpus
nltk.download('brown')

words = brown.words(categories='fiction')
print(words[:10])
```
4. **Output:**
   
   ```['Thirty-three', 'Scotty', 'did', 'not', 'go', 'back', 'to', 'school', '.', 'His']```
5. **Conclusion:**
   
   Successfully implemented Python program using the Brown Corpus.
   

### Using the Penn Treebank Corpus:
1. **Aim:** Implement a program to use the Penn Treebank Corpus.
   
2. **Requirements:**
    * Python 3.7 or above
    * nltk library
      
3. **Program:**
```python
import nltk
from nltk.corpus import treebank

# Download necessary corpus
nltk.download('treebank')

# Display a sentence from the corpus
print(treebank.parsed_sents('wsj_0001.mrg')[0])
```
4. **Output:**
 ```
(S
  (NP-SBJ
    (NP (NNP Pierre) (NNP Vinken))
    (, ,)
    (ADJP (NP (CD 61) (NNS years)) (JJ old))
    (, ,))
  (VP
    (MD will)
    (VP
      (VB join)
      (NP (DT the) (NN board))
      (PP-CLR (IN as) (NP (DT a) (JJ nonexecutive) (NN director)))
      (NP-TMP (NNP Nov.) (CD 29))))
  (. .))
```
5. **Conclusion:**
   
   Successfully implemented Python program using the Penn Treebank Corpus.

### 6. Questions:
   
   **Q1. Define brown corpus. What’s the main feature of brown corpus?**
   
   * The Brown Corpus is a one-million-word collection of American English texts compiled at Brown University in 1961 by Kucera and Francis.  
   * main feature: It is balanced, containing 500 samples from diverse genres (news, fiction, academic writing, etc.) to represent general written English of the 1960s.
   
   **Q2. What's the difference between brown corpus and penn treebank corpus?**
   
   | **Aspect**        | **Brown Corpus**         | **Penn Treebank**                 |
| ----------------- | ------------------------ | --------------------------------- |
| **Year / Origin** | 1961, Brown University   | 1990s, University of Pennsylvania |
| **Size**          | ~1 million words         | ~4.5 million words                |
| **Content**       | Balanced written English | Mainly Wall Street Journal text   |
| **Purpose**       | Study of general English | NLP parser training               |
