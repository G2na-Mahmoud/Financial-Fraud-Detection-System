# AI-Driven Financial Fraud Detection System 🚀

**Description:**
A comprehensive machine learning pipeline designed to detect fraudulent mobile money transactions. The system analyzes over 6.3 million records with **99.9% accuracy** and utilizes PCA to optimize performance, reducing processing time by 45%.

---

## 🛠️ Project Workflow & Widgets (Orange Data Mining)

### 1️⃣ Phase: Data Entry & Exploration 📥
| Widget | Function | Technical Logic |
| :--- | :--- | :--- |
| **File** 📄 | Data loading point | Defined column types and set the Target variable (isFraud). |
| **Data Info** ℹ️ | Quick data summary | Verified the successful upload of 6.3M records and 11 features. |
| **Data Table** 📋 | Manual data review | Conducted a sanity check to ensure data integrity before analysis. |

### 2️⃣ Phase: Preprocessing Pipeline ⚙️
| Widget | Function | Technical Logic |
| :--- | :--- | :--- |
| **Impute** 🩹 | Missing values handling | Filled gaps with mean values to ensure model stability. |
| **Normalize** 📏 | Scaling features | Unified numeric ranges (0 to 1) to prevent feature dominance. |
| **Continuize** 🔢 | Categorical encoding | Used One-Hot Encoding to transform text (e.g., TRANSFER) into math vectors. |

### 3️⃣ Phase: Feature Selection & Engineering 🎯
| Widget | Function | Technical Logic |
| :--- | :--- | :--- |
| **Rank** 🏆 | Feature importance scoring | Identified "Balance Gap" as the strongest indicator of fraud. |
| **Select Columns** 🔍 | Dimensionality filtering | Removed noise by keeping only the most influential variables. |

### 4️⃣ Phase: Data Visualization 📊
| Widget | Function | Technical Logic |
| :--- | :--- | :--- |
| **Distributions** 📉 | Data pattern analysis | Discovered that 100% of fraud occurs in TRANSFER & CASH_OUT types. |
| **Scatter Plot** 📍 | Variable relationship mapping | Revealed that in 99% of fraud cases, the victim's balance reaches 0.00. |
| **Box Plot** 📦 | Outlier detection | Distinguished between "Wealthy Users" and "Fraudulent Drainers." |

### 5️⃣ Phase: Dimensionality Reduction 💎
| Widget | Function | Technical Logic |
| :--- | :--- | :--- |
| **PCA** ⚡ | Computational optimization | Reduced features to 3-5 components, speeding up training by 45%. |
| **Correlation** 🔗 | Relationship measurement | Analyzed the strong link between transaction amounts and fraud flags. |

### 6️⃣ Phase: Modeling & Evaluation 🤖
| Widget | Function | Technical Logic |
| :--- | :--- | :--- |
| **Data Sampler** ✂️ | Training/Testing split | Ensured the model learned general rules rather than memorizing samples. |
| **Random Forest** 🌳 | (The Champion) Ensemble model | Handled the extreme "Class Imbalance" (rare fraud cases) perfectly. |
| **Test and Score** ✅ | Performance benchmarking | Evaluated all models to reach the final 99.9% accuracy. |
| **Confusion Matrix** 📋 | Detailed error analysis | Focused on "High Recall" to ensure no fraudster goes undetected. |
| **ROC Curve** 📈 | Classification efficiency | Demonstrated high precision in catching fraud without bothering legal users. |

---

## 🏆 Final Results
* **Accuracy:** 99.9% ✨
* **Efficiency:** 45% Faster Training 🏎️
* **Key Signature:** Account Clearing behavior (0.00 Final Balance) 💸
