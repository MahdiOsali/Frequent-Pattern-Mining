# Frequent-Pattern-Mining
# Market Basket Analysis using Apriori & FP-Growth

This repository contains a complete implementation of **Frequent Itemset Mining** and **Association Rule Learning** using Python. The project demonstrates the entire workflow: data preprocessing, converting raw transactions into a one-hot encoded matrix, mining frequent itemsets using two classic algorithms (Apriori and FP-Growth), and extracting powerful association rules.

---

## 📌 Project Overview

Market Basket Analysis (MBA) is a fundamental technique in data mining used to discover patterns, co-occurrences, and relationships between items in large transactional datasets. This project applies:

* **Apriori Algorithm**
* **FP-Growth Algorithm**
* **Association Rule Mining** (support, confidence, lift, conviction, etc.)

We also compare both algorithms in terms of:

* Runtime
* Number of frequent itemsets
* Number of rules generated


---

## 🚀 Features

* Clean & reproducible workflow
* Transactional dataset cleaning
* One-hot encoded matrix generation
* Apriori frequent itemset mining
* FP-Growth frequent itemset mining
* Rule extraction using `mlxtend.association_rules`

---

## 🧠 Algorithms Explained

### **Apriori Algorithm**

Apriori works by generating candidate itemsets and pruning those with insufficient support. It follows the **downward closure property**, meaning if an itemset is infrequent, all its supersets are also infrequent.

### **FP-Growth Algorithm**

FP-Growth avoids candidate generation and instead builds a compressed structure called an **FP-Tree**. It is significantly faster and more scalable, especially on large dense datasets.

---

## 🛠️ Tools & Libraries

* Python 3.x
* Pandas
* NumPy
* Mlxtend
* Jupyter Notebook

---

## 📊 Comparison Summary

| Metric                | Apriori                      | FP-Growth                     |
| --------------------- | ---------------------------- | ----------------------------- |
| **Runtime**           | Slower (multiple DB scans)   | Much faster (only 2 DB scans) |
| **Frequent Itemsets** | Similar output               | Similar output                |
| **Rules Generated**   | Same as FP-Growth            | Same as Apriori               |
| **Scalability**       | Weak on large dense datasets | Excellent scalability         |

---


## 📄 License

MIT License.

---

## 🤝 Contributing

Feel free to submit issues or pull requests to improve this project.

---

This project uses the `mlxtend.frequent_patterns` module for Apriori, FP-Growth, and association rules.
