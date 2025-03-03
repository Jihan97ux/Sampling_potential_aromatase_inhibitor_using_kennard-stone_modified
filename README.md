# Selection of Potential Aromatase Inhibitors Using Fingerprint Analysis and pIC50 Integrated with the Kennard-Stone Algorithm  

## Author   
**Jihan Fadila** (105222022)  
📧 Email: jihan4han97@gmail.com

---

## 📌 Introduction  
Breast cancer remains a significant global health issue, with **2.3 million cases worldwide**, accounting for **11.7% of all cancer cases**. In Indonesia, it is the most prevalent cancer, with **68,858 cases and over 22,000 deaths** annually.  

The key factor in **breast cancer progression** is the **dysregulation of estrogen levels** facilitated by the **aromatase enzyme**. Aromatase inhibitors (**AIs**) have been widely used to suppress estrogen production. However, existing AIs often cause **cardiovascular issues and bone density loss**.  

This study employs **molecular fingerprint analysis** and **pIC50 bioactivity values** to identify potential **aromatase inhibitors**. Additionally, the **Kennard-Stone algorithm** is integrated to ensure a **representative selection of compounds** from a large dataset.  

---

## 🎯 Research Objectives  
1. **Identify** potential aromatase inhibitor compounds with high **pIC50 values**.  
2. **Implement** the **Kennard-Stone algorithm** to select a diverse and representative dataset.  
3. **Evaluate** the effectiveness of the selected compounds through **molecular docking**.  

---

## 🧪 Methodology  
### **1. Dataset Collection & Preprocessing**  
- The dataset consists of **1,400 aromatase inhibitor compounds**.  
- Features were extracted using **PaDEL Descriptor**, producing **substructure fingerprints**.  
- Only compounds with **pIC50 ≥ 6.5** and **MW ≤ 300 Da** were selected.  

### **2. Kennard-Stone Algorithm for Sample Selection**  
- Ensures **diverse molecular structures** are included.  
- Prioritizes compounds with **high pIC50 values**.  
- Distributes samples **evenly in feature space** for unbiased selection.  

### **3. Molecular Processing**  
- **SMILES representations** were converted into **PDB files** using **RDKit**.  
- **Geometric optimization** was applied using **Universal Force Field (UFF)**.  
- **3D Molecular Visualization** was performed using **Py3Dmol**.  

### **4. Computational Complexity Analysis**  
- Algorithm time complexity: **O(m² * n)**, where **m** = number of samples, **n** = number of features.  
- Euclidean distance calculations and **feature normalization** were implemented to improve efficiency.  

---

## 📊 Results & Discussion  
### **Data Selection & Kennard-Stone Sampling**  
- **203 compounds** were selected based on **pIC50, MW, and hydrogen bonding criteria**.  
- **30 samples** were chosen using the **modified Kennard-Stone algorithm** with:  
  - **40% weighting on pIC50 values**.  
  - **60% weighting on data variation (fingerprint features)**.  
- The final selection maintained a **diverse structural representation**.  

### **Computational Performance**  
- Execution time: **0.0311 seconds** (Google Colaboratory).  
- **Robust feature scaling** ensured fair data distribution before sample selection.  

### **3D Visualization of Selected Compounds**  
- **203 optimized molecular structures** were successfully visualized using **Py3Dmol**.  
- Structures were analyzed for **functional interactions with biological targets**.  

---

## 📌 Conclusion  
- The **modified Kennard-Stone algorithm** effectively selected diverse **high-pIC50 compounds**.  
- **Molecular fingerprint analysis** provided critical insights into **structure-activity relationships (SAR)**.  
- The selected compounds can serve as **potential candidates for aromatase inhibition** in breast cancer treatment.  

Future work includes **molecular docking simulations** and **machine learning-based drug discovery**.  
