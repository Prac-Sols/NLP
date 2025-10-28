
## Exp 4
1. **Aim:** Write program for POS tagging on the given text.
   
2. **Requirements:**
    * Computer system with an intel i3/i5 CPU or above, and 4GB of ram or above.
    * Python 3.7 or above
    * nltk library
  
3. **Program:**
```python
import nltk
from nltk.tokenize import word_tokenize

nltk.download('punkt')
nltk.download('averaged_perceptron_tagger')

text = "The quick brown fox jumps over the lazy dog"
tokens = word_tokenize(text)

# POS Tagging
pos_tags = nltk.pos_tag(tokens)
print("\nPOS Tagging Results:")
for word, tag in pos_tags:
    print(f"{word} -> {tag}")
```

4. **Output:**
```
POS Tagging Results:
The -> DT
quick -> JJ
brown -> NN
fox -> NN
jumps -> VBZ
over -> IN
the -> DT
lazy -> JJ
dog -> NN
```

5. **Conclusion:**
   Successfully implemented Python program for POS tagging on the given text.

6. **Questions:**
    1. **What is the role of the word_tokenize() function in the POS tagging program?**
  
       The role of word_tokenize() is to split the text into individual words or tokens..
  
    2. **Why do we use nltk.download('averaged_perceptron_tagger') before performing POS tagging?**
   
        * NLTK’s POS tagger uses a pre-trained model called the Averaged Perceptron Tagger.  
        * Running nltk.download('averaged_perceptron_tagger') downloads this model so your program can assign POS tags.
