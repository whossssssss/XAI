# Social media text analysis for psycho-emotinal expressions of sentiment, emotions, intent, manipulation and cognitive distortions in social media for Chinese

## Abstract

This research develops an interpretable AI-based system for analyzing Chinese social media text, specifically designed to detect psycho-emotional expressions, sentiment, intent, manipulation, and cognitive distortions. Through the construction of targeted n-gram dictionaries and feature engineering methods, we achieved detection of 10 cognitive distortion patterns, with a 51.4% detection rate on 863 Chinese text samples.

## Research Background

### Prior Art Review

#### 1. Social Media Sentiment Analysis
- **Traditional Methods**: Lexicon-based sentiment analysis
- **Machine Learning Approaches**: SVM, Random Forest classifiers
- **Deep Learning Methods**: BERT, RoBERTa pre-trained models

#### 2. Cognitive Distortion Detection
- **Psychological Foundation**: Beck's Cognitive Behavioral Theory
- **Existing Tools**: Cognitive distortion detection tools in English
- **Chinese Research**: Limited research on Chinese cognitive distortion detection

#### 3. Explainable AI in NLP
- **LIME, SHAP**: Model interpretability tools
- **Attention Mechanisms**: Visualizing model focus points
- **Rule-based Systems**: Dictionary-based interpretable methods

## Research & Development Work

### 1. Data Collection and Construction
```python
# Dataset Composition
datasets = {
    'weibo': 700 texts,          # Real Weibo data
    'mental_filtering': 60 texts, # Targeted cognitive distortion data
    'personalization': 75 texts,  # Personalization distortion data
    'other_distortions': 28 texts # Other distortion types
}
```

### 2. Methodological Innovations

#### 2.1 Targeted Feature Engineering
- **77 n-gram features** across 10 cognitive categories
- **Weighted scoring system** with explainable weights
- **Specialized dictionaries** for Chinese linguistic patterns

#### 2.2 Cognitive Distortion Taxonomy
We defined and implemented detection for 10 cognitive distortion types:
1. **Mental Filtering** - Selective attention to negative aspects
2. **Personalization** - Excessive self-blame
3. **Overgeneralization** - Broad negative conclusions
4. **Catastrophizing** - Expecting the worst-case scenario
5. **Labeling** - Global negative self-evaluation
6. **Mind Reading** - Assuming others' negative thoughts
7. **Emotional Reasoning** - Believing emotions reflect reality
8. **Should Statements** - Rigid demands on self/others
9. **Magnification** - Exaggerating negative aspects
10. **Minimization** - Downplaying positive aspects

### 3. Technical Implementation

#### 3.1 System Architecture
```
Data Loading → Text Preprocessing → Feature Engineering → Analysis → Visualization
```

#### 3.2 Core Algorithms
```python
class TargetedNgramDictionary:
    """Explainable feature extraction using targeted n-grams"""
    
    def extract_explainable_features(self, text_tokens):
        # Feature extraction with transparent scoring
        pass
```

## Research Results

### 1. Performance Metrics

#### Detection Rates
| Feature Category | Detection Rate | Average Score |
|------------------|----------------|---------------|
| Manipulation Intent | 48.2% | 0.389 |
| Unclassified Distortions | 47.7% | 0.416 |
| Positive Sentiment | 35.2% | 0.270 |
| Labeling Distortion | 12.5% | 0.211 |

#### Cognitive Distortion Statistics
- **Overall Detection**: 51.4% of texts contain ≥1 distortion
- **High-Risk Texts**: 35.9% contain ≥2 distortion types
- **Most Prevalent**: Overgeneralization (24.8%)

### 2. Key Findings

#### 2.1 Feature Correlations
- Strong correlation between catastrophizing and labeling (r=0.975)
- Manipulation intent positively correlates with positive sentiment (r=0.793)
- Negative correlation between manipulation and overgeneralization (r=-0.546)

#### 2.2 Platform Analysis
- **Weibo**: Highest manipulation scores (0.457)
- **Mental Filtering Dataset**: Targeted detection success (0.225)
- **Personalization Dataset**: Lower than expected detection rates

### 3. Reproducibility
- Complete code and data preprocessing pipelines

## Comparative Analysis

### Advantages Over Existing Methods

| Aspect | Traditional Methods | Our Approach |
|--------|---------------------|--------------|
| **Interpretability** | Black-box models | Transparent feature scoring |
| **Chinese Specificity** | Limited adaptation | Targeted Chinese n-grams |
| **Cognitive Focus** | General sentiment | Specific distortion types |
| **Deployment** | Complex infrastructure | Lightweight, rule-based |

### Limitations and Challenges
1. **Detection Rate Variance**: Some features show low detection rates
2. **Data Scale**: Limited to 863 texts for initial validation
3. **Language Specificity**: Focused on Chinese, requires adaptation for other languages

## Theoretical Contributions

### 1. Psycholinguistic Insights
- Identified Chinese-specific cognitive distortion patterns
- Developed weighted scoring for distortion severity
- Established baseline metrics for Chinese social media

### 2. Technical Innovations
- Explainable AI approach for psychological analysis
- Hybrid rule-based and statistical methodology
- Scalable feature engineering framework

## Practical Applications

### 1. Mental Health Monitoring
- Early detection of cognitive distortion patterns
- Automated screening for at-risk individuals
- Support for mental health professionals

### 2. Content Moderation
- Identification of manipulative content
- Detection of harmful psychological patterns
- Enhanced platform safety measures

## References

1. Social Media Sentiment Analysis for Cryptocurrency Market Prediction
2. Causal Analysis of Generic Time Series Data Applied for Market Prediction
3. Associating cognitive distortions to social context and relationships in psychological conversation data
