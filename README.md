# **Automated GDPR Compliance Checker Using Selenium**
### **Evaluating GDPR Compliance of Educational Websites - (January 2025)**  
### **A Research Project in Collaboration with Princess Sumaya University for Technology (PSUT)**  

## **Project Overview**  
This repository contains a **fully automated GDPR compliance checker** that directly visits each website in the dataset, detects cookie banners, interacts with consent buttons, and logs compliance data.

This approach was developed to **overcome the limitations of the 2GDPR scraper** and allows **direct large-scale GDPR auditing** across **8,483 educational websites**, derived from **[The Majestic Million](https://majestic.com/reports/majestic-million?domain=&majesticMillionType=2&tld=paris&oq=&canUseDefault=)** dataset.

### **Project Contributors**  
- **Sana Mourad & Aya Aljabali** – Research & dataset selection.
- **Yousef Jarbou** – Automation & implementation.
- **Dr. Mu'awya Al-Dala'ien** – Supervision.

---

## **How the GDPR Compliance Checker Works**
1. **Directly visits each website** from our dataset.
2. **Detects cookie consent banners** automatically using **advanced XPath selectors**.
3. **Identifies & interacts with consent buttons**:
   - **“Accept All”**, **“Reject All”**, and **Granular Consent Options**.
4. **Captures Cookies Before & After Consent**:
   - Collects cookies **before clicking the consent button**.
   - Collects cookies **after clicking the consent button**.
   - **Compares the difference** to check if cookies are set **before consent is given**.
5. **Logs and stores results in a structured format**:
   - **Website URL**
   - **Compliance Status** (Compliant, Non-Compliant, Partially Compliant)
   - **Granular Consent Availability**
   - **Number of Cookies Before & After Consent**

---

## **Challenges & How We Optimized the Process**

### **1.Overcoming the Lack of a Scalable GDPR Compliance Tool**
Overcame the challenge of not finding a freely available tool capable of handling large-scale GDPR compliance checks by developing our own fully automated solution, ensuring efficiency, scalability, and accuracy in analyzing 8,453 websites.
 
### **2.Optimizing Processing Time**
To handle the large dataset efficiently:
- **Batch Processing**:
  - The dataset was split into **43 batches**, each containing **200 URLs**.
  - Each batch took approximately **1.5 hours** to process.
- **Parallel Execution**:
  - Ran batches across **three different devices**, each handling **14 browser tabs in parallel**.
  - This strategy allowed us to process the entire dataset of **8,453 websites in under 2 hours**.
### **3. Dynamic Content & Hidden Consent Mechanisms**
- Some websites loaded banners asynchronously or buried consent options in deep menus.
- **Solution:**  
  - Used **explicit waits & JavaScript execution** to handle delays.
  - Implemented **deep search logic** to locate hidden consent elements.


---
## **Final Results**
- **Successfully analyzed 8,453 websites.**
-  **Identified major trends in non-compliance, such as setting cookies before consent.**
- **Overcame the challenge of not finding a freely available tool capable of handling large-scale GDPR compliance checks by developing our own fully automated solution, ensuring efficiency, scalability, and accuracy in analyzing 8,453 websites** 
