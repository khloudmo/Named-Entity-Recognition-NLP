#  Named Entity Recognition (NER) from News Articles  

##  Project Overview  
This project focuses on **Named Entity Recognition (NER)** — identifying entities like **people, locations, and organizations** from text data using both **rule-based** and **model-based** approaches.  

### Goal
- Extract entities such as People, Locations, and Organizations.  
- Compare rule-based and model-based (SpaCy) NER approaches.  
- Visualize and analyze entity extraction performance.  

---

## Dataset
- **Source:** [CoNLL2003 Dataset (Kaggle)](https://www.kaggle.com/datasets/alaakhaled/conll003-english-version)  
- Contains sentences annotated with named entities (PER, LOC, ORG, MISC).  
- Split into:  
  - `train.txt`  
  - `valid.txt`  
  - `test.txt`  

---

## Tools & Libraries
- Python  
- SpaCy  
- Pandas  
- Matplotlib  

---

## Workflow

1. **Load Dataset**  
   - Read CoNLL2003 formatted text files (`train.txt`, `valid.txt`, `test.txt`).  

2. **Rule-based NER**  
   - Used regular expressions (Regex) to detect simple patterns like names or common organizations.  

3. **Model-based NER (SpaCy)**  
   - Used two SpaCy models:  
     - `en_core_web_sm` (small model)  
     - `en_core_web_md` (medium model)  
   - Compared their performance.  

4. **Visualization**  
   - Displayed extracted entities using **displacy**.  
   - Created a **bar chart** comparing number of detected entities per model.  

---

## Results

| Model | Entities Detected | Performance |
|--------|--------------------|--------------|
| **Rule-based** | Very limited | Detects only simple patterns |
| **SpaCy (en_core_web_sm)** | Moderate | Lightweight, decent accuracy |
| **SpaCy (en_core_web_md)** | Best | Detects more entities with higher accuracy |

### Visualization
- Entity highlights shown using **displacy**  
- Comparison chart showing number of entities per model  

---

## Conclusion
- The **rule-based** method is simple but lacks accuracy.  
- The **SpaCy medium model (`en_core_web_md`)** provides the most accurate and detailed entity extraction.  
- Recommended for practical NER tasks.  

---

## Future Work
- Try larger models like `en_core_web_trf` (Transformer-based).  
- Evaluate performance quantitatively (Precision, Recall, F1).  
- Apply on real-world news datasets or social media data.  

---

## Author
**Khloud Mohamed Ibrahem Ali**  
Computer Science (AI Major)  
🔗 [GitHub](https://github.com/khloudmo) | [LinkedIn](https://www.linkedin.com/in/kholoud-mohamed-07-I)
