# 🔒 Intrusion Detection System Research

## 📊 Overview 

This repository holds the findings and research from our project on **Adaptive Intrusion Detection Systems (IDS)**, which secured **7th place** at the **TCCD Research Day** competition. 🥳✨ 

Our study focuses on developing a statistical and machine learning-based IDS that detects novel cyber threats by analyzing deviations from normal network behavior in real time. 🤖⚠️

## 📜 Abstract 

In an era of growing cybersecurity threats, intrusion detection systems (IDS) play a critical role in safeguarding networks. However, traditional IDS often fail to detect novel attacks due to their reliance on static signatures. This research proposes an adaptive, data-driven IDS that uses statistical methods and machine learning algorithms to identify anomalies in real time by modeling baseline network behavior. 

The study utilizes the **RRE-KDD dataset**, featuring over 148,000 events and 37 types of attacks (e.g., DoS, U2R). By leveraging descriptive statistics, statistical thresholds, and the **Random Forest** algorithm, our system achieves improved threat detection performance. The results demonstrate the effectiveness of our approach in detecting cyber intrusions with higher accuracy and reduced error rates.

## 📂 Dataset 

### **RRE-KDD Dataset**
- **Comprehensive Network Traffic Collection**
- **Attack Types:** 37 (e.g., DoS, U2R, etc.)
- **Key Variables:** Protocol type, service, source/destination bytes, and more.
- **Training Set:** 126,000 events
- **Testing Set:** 22,000 events

## ⁉️ Research Questions

1. **Descriptive Statistics for Baseline Patterns:**
   - How can measures like mean, median, and variance define \"normal\" network behavior, creating a foundation for anomaly detection?

2. **Effective Statistical Thresholds:**
   - What thresholds (e.g., standard deviations, percentiles) are most effective for flagging anomalies in network traffic?

3. **Z-Score vs. Percentile Thresholds:**
   - How does Z-score analysis compare to percentile-based thresholds in detecting network intrusions?

4. **Time-Series Techniques for Anomaly Detection:**
   - Can moving average and exponential smoothing methods detect time-based anomalies in network traffic?

5. **Statistical Hypothesis Testing:**
   - How can methods like the Chi-square test identify significant deviations in network traffic patterns?


## 🔬 Methodology 

### 🌲 **Random Forest Algorithm** 

Random Forest is an ensemble learning method that builds multiple decision trees and combines their outputs for improved accuracy and robustness.

#### Mathematical Representation
```math
Given\ N\ decision trees\ (\ h_1(x), h_2(x),\ldots, h_N(x)\ ),\ the\ final\ result\ is:
```

```math
Classification:\ [\hat{y} = \text{mode}(h_i(x))\ ]
```
```math
Regression:\ [\hat{y} = \frac{1}{N} \sum_{i=1}^N h_i(x)\ ]
```
Each tree is trained on a bootstrapped sample of the dataset and splits nodes based on **Gini impurity** (\(G\)):
```math
 [G = 1 - \sum_{i=1}^C p_i^2\ ]
```
```math
Where:
\ (p_i)\ is\ the\ probability\ of\ class\ (i),
\ (C)\ is\ the\ total\ number\ of\ classes.
```
## 🔍 Key Findings
- **Descriptive Statistics:** Established robust baseline network behavior patterns, enabling effective anomaly detection.
- **Statistical Thresholds:** Percentile-based thresholds showed higher accuracy compared to Z-score analysis for flagging anomalies.
- **Time-Series Techniques:** Moving averages effectively detected time-based anomalies, such as traffic spikes.
- **Random Forest:** Achieved high detection accuracy with minimal false positives by leveraging ensemble learning.

## 📝 Conclusion
This project highlights the potential of adaptive, statistical, and machine learning-based IDS in addressing modern cybersecurity challenges. By combining statistical techniques and Random Forest algorithms, we significantly enhanced the detection accuracy of network intrusions while maintaining low false positive rates. Our findings pave the way for more advanced, real-time threat detection systems.

---
## 👥 Team
<table>
<tr>
    <td align="center">
        <a href="https://github.com/Amrhanysayed">
            <img src="https://github.com/Amrhanysayed.png" width="100px;" alt="Amr Hany"/><br />
            <sub><b>Amr Hany</b></sub>
        </a><br />
    </td>
    <td align="center">
          <a href="https://github.com/xx-Tasneem-Ahmed-xx">
              <img src="https://github.com/xx-Tasneem-Ahmed-xx.png" width="100px;" alt="Tasneem Ahmed"/><br />
              <sub><b>Tasneem Ahmad</b></sub>
          </a><br />
      </td>
    <td align="center">
        <a href="https://github.com/bedosaber77">
            <img src="https://github.com/bedosaber77.png" width="100px;" alt="Abdelrahman Medhat"/><br />
            <sub><b>Abdelrahman Medhat</b></sub>
        </a><br />
    </td>
    <td align="center">
        <a href="https://github.com/Hussein-Mohamed1">
            <img src="https://github.com/Hussein-Mohamed1.png" width="100px;" alt="Hussein Mohamed"/><br />
            <sub><b>Hussien Mohamed</b></sub>
        </a><br />
    </td>
     <td align="center">
        <a href="https://github.com/KarimmYasser">
            <img src="https://github.com/KarimmYasser.png" width="100px;" alt="Karim Yasser"/><br />
            <sub><b>Karim Yasser</b></sub>
        </a><br />
    </td>
 <td align="center">
        <a href="https://github.com/exo1i">
            <img src="https://github.com/exo1i.png" width="100px;" alt="Youssef Noser"/><br />
            <sub><b>Youssef Noser</b></sub>
        </a><br />
    </td>
</tr>
</table>
