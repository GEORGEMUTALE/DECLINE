# <span style="color:#2A4D9B;">Cognitive Decline Factors – Dataset Evaluation Report</span>

This report provides evaluation of multiple datasets relevant to modelling **pre-clinical factors related to cognitive decline**.  
Each dataset is assessed based on its provenance, sample size, advantages, limitations, and suitability for early-risk modelling.

---

# <span style="color:#1B7F5F;">1. Stress Detection Dataset</span>

**Source:** https://www.kaggle.com/datasets/swadeshi/stress-detection-dataset  
**Sample Size:** 3,000 (100 participants × 30 days)  
**Data Type:** Daily stress levels  
**Origin:** <span style="color:#C0392B;">Undefined</span>

### <span style="color:#2471A3;">Advantages</span>
- Contains temporal/streak-based stress data, helpful for behavioural modelling.
- Reasonable sample size for exploratory analysis.
- Stress is strongly associated with early cognitive decline.

### <span style="color:#C0392B;">Weaknesses</span>
- No documentation on data collection methodology.
- No demographic details included.

---

# <span style="color:#1B7F5F;">2. Alzheimer’s Disease Dataset</span>

**Source:** https://www.kaggle.com/datasets/rabieelkharoua/alzheimers-disease-dataset  
**Sample Size:** 2,149  
**Type:** Clinical features  
**Origin:** Synthetic  
**Important Note:** Contains *post-diagnosis* cognitive decline data.

### <span style="color:#2471A3;">Advantages</span>
- Rich set of health and diagnostic indicators.
- Useful for understanding Alzheimer's patterns in diagnosed individuals.

### <span style="color:#C0392B;">Weaknesses</span>
- Does *not* support pre-clinical or preventive modelling.
- Synthetic: may not match real physiological distributions.
- Limited relevance for early-cognitive-risk research.

---

# <span style="color:#1B7F5F;">3. Human Cognitive Performance Dataset</span>

**Source:** https://www.kaggle.com/datasets/samxsam/human-cognitive-performance-analysis  
**Sample Size:** 80,000  
**Type:** Cognitive performance scores  
**Origin:** <span style="color:#C0392B;">Undefined</span>

### <span style="color:#2471A3;">Advantages</span>
- Very large dataset → suitable for deep learning or robust modelling.
- Multiple variables linked to cognitive testing.
- Useful for establishing baseline cognitive-performance patterns.

### <span style="color:#C0392B;">Weaknesses</span>
- No verification of authenticity or methodology.
- Demographic and sampling details are missing.
- Potential synthetic or noisy features due to insufficient documentation.

---

# <span style="color:#1B7F5F;">4. Anemia / B12 Deficiency Dataset</span>

**Source:** https://www.kaggle.com/datasets/serhathoca/anemia-disease  
**Sample Size:** 15,300  
**Type:** Clinical blood-test results  
**Origin:** Real medical dataset (Turkey, 2013–2018)

### <span style="color:#2471A3;">Advantages</span>
- Real-world patient data → high reliability.
- B12 deficiency is known to cause neurological and cognitive impairment.
- Large, multi-year dataset supports longitudinal insights.

### <span style="color:#C0392B;">Weaknesses</span>
- Region-specific population → may affect generalizability.
- Only hematological data; lacks lifestyle/psychological features.
- Confounding variables (diet, sleep, stress) not included.

---

# <span style="color:#1B7F5F;">5. Anxiety Levels Dataset</span>

**Source:** https://www.kaggle.com/datasets/natezhang123/social-anxiety-dataset  
**Sample Size:** 10,000+  
**Type:** Survey + behavioral indicators  
**Origin:** Australia (real survey data)  
**Contains:** Enhanced + Family Anxiety datasets

### <span style="color:#2471A3;">Advantages</span>
- Real-world psychological data with environmental context.
- Large sample size with varied anxiety severity levels.
- Anxiety and stress major pre-clinical cognitive-decline predictor.
- Family-anxiety dataset adds intergenerational and social dimension.
- Region-specific (Australia).

### <span style="color:#C0392B;">Weaknesses</span>
- Subject to self-reporting bias because Australia may not well represent the people from Europe 
- No personality trait items

---

# <span style="color:#1B7F5F;">6. Student Depression Dataset</span>

**Source:** https://www.kaggle.com/datasets/hopesb/student-depression-dataset/data  
**Sample Size:** 27,901  
**Type:** Mental health (survey)  
**Origin:** Synthetic

### <span style="color:#2471A3;">Advantages</span>
- Large dataset with depression-related variables.
- Useful for assessing psychological precursors to cognitive stress.

### <span style="color:#C0392B;">Weaknesses</span>
- Synthetic → limited realism.
- Focuses only on students; poor generalization 
- No clinical verification.

---

# <span style="color:#1B7F5F;">7. Sleep Health & Lifestyle Dataset</span>

**Source:** https://www.kaggle.com/datasets/uom190346a/sleep-health-and-lifestyle-dataset  
**Sample Size:** 400  
**Type:** Lifestyle + sleep quality  
**Origin:** Synthetic

### <span style="color:#2471A3;">Advantages</span>
- Includes key pre-clinical factors: sleep, stress, exercise.
- Clean and easy to work with.
- Useful for prototyping or small-scale models.

### <span style="color:#C0392B;">Weaknesses</span>
- Very small sample size → low statistical power.
- Synthetic → limits real-world applicability.

---

# <span style="color:#9B59B6;">Dataset Comparison Table</span>

| Dataset | Size | Data Origin | Real/Synthetic | Strength | Limitation |
|--------|------|-------------|----------------|----------|------------|
| Stress Detection | 3,000 | Undefined | Unknown | Temporal stress patterns | No demographic info |
| Alzheimer’s | 2,149 | Synthetic | Synthetic | Rich clinical features | Post-diagnosis only |
| Cognitive Performance | 80,000 | Undefined | Unknown | Very large dataset | Unverified origin |
| B12 Anemia | 15,300 | Turkey medical records | Real | Clinically reliable | Misses Personality trait items |
| Anxiety Levels | 11,000 | Australia surveys | Real | High psychological relevance | Survey bias |
| Student Depression | 27,901 | Synthetic | Synthetic | Large mental health dataset | Student-only |
| Sleep Health | 400 | Synthetic | Synthetic | Good feature variety | Very small dataset |

---

# <span style="color:#2A4D9B;">Conclusion</span>

Among all datasets evaluated, **the Anxiety Levels dataset** offers the strongest and most credible foundations for modelling **pre-clinical cognitive decline risk** due to their real-world origin, sample size, and it also contains a column having stress levels.

**Stress Detection dataset** only contains the personality trait items but **the Cognitive Performance dataset** as many samples and contains the lifestyle factors though it is synthetic and has no Personality trait items 


My final dataset is **the Anxiety Levels Dataset**

---