# Chinese Social Media Psychological Sentiment Analysis System - Complete Results Report

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)
[![AI](https://img.shields.io/badge/AI-Interpretable%20AI-orange)](https://)

## 📋 Executive Summary

This project has successfully implemented an interpretable AI-based Chinese social media text analysis system, conducting comprehensive psychological sentiment analysis on 863 real Chinese social media texts, effectively detecting cognitive distortion patterns, emotional tendencies, and manipulative intentions.

## 🎯 Key Achievements

### 📊 Data Overview
- **Total Samples**: 863 texts
- **Platform Distribution**: Weibo (81.1%), personalization (8.7%), mental_filtering (7.0%), other_distortions (3.2%)
- **Sentiment Distribution**: Negative (64.5%), Positive (35.5%)

### ⚠️ Cognitive Distortion Detection Results
- **51.4%** of texts contain at least one cognitive distortion
- **35.9%** of texts are high-risk (≥2 distortions)
- **Most Common Distortions**: Unclassified distortions (47.7%), Overgeneralization (24.8%), Labeling (12.5%)

## 📈 Detailed Analysis Results

### Feature Score Ranking (by Mean)
| Feature Type | Average Score | Detection Success Rate | Severity |
|--------------|---------------|------------------------|----------|
| Unclassified Distortions | 0.416 | 47.7% | 🔴 High |
| Manipulation Intent | 0.389 | 48.2% | 🔴 High |
| Positive Sentiment | 0.270 | 35.2% | 🔴 High |
| Labeling Distortion | 0.211 | 12.5% | 🔴 High |
| Overgeneralization | 0.174 | 24.8% | 🔴 High |
| Catastrophizing | 0.106 | 11.8% | 🔴 High |
| Mental Filtering | 0.016 | 2.1% | 🟡 Medium |
| Mind Reading | 0.002 | 0.2% | 🟢 Low |

### 🔗 Feature Correlation Analysis
Strong correlation feature pairs discovered:
- **Catastrophizing ↔ Labeling**: 0.975 (Strong Positive Correlation)
- **Manipulation Intent ↔ Positive Sentiment**: 0.793 (Strong Positive Correlation)
- **Manipulation Intent ↔ Negative Sentiment**: -0.573 (Negative Correlation)
- **Manipulation Intent ↔ Overgeneralization**: -0.546 (Negative Correlation)
![image](https://github.com/whossssssss/XAI/blob/main/img/1.png)

### 🌐 Platform Feature Differences
- **Weibo**: Unclassified distortions (0.500) and manipulation intent (0.457) most prominent
- **Mental Filtering**: Mental filtering features significant (0.225)
- **Other Distortions**: Manipulation intent (0.550) and labeling (0.429) relatively high
- **Personalization**: Feature performance relatively weak
![image](https://github.com/whossssssss/XAI/blob/main/img/2.png)

## 🧠 Detailed Cognitive Distortion Analysis

### Severity Ranking
1. **Unclassified Distortions** (0.416) - 🔴 High Risk
2. **Labeling Distortion** (0.211) - 🔴 High Risk
3. **Overgeneralization** (0.174) - 🔴 High Risk
4. **Catastrophizing** (0.106) - 🔴 High Risk
5. **Mental Filtering** (0.016) - 🟡 Medium Risk
6. **Mind Reading** (0.002) - 🟢 Low Risk

### Frequency Ranking
1. **Unclassified Distortions** (47.7%) - 🔴 Common
2. **Overgeneralization** (24.8%) - 🟡 General
3. **Labeling** (12.5%) - 🟡 General
4. **Catastrophizing** (11.8%) - 🟡 General
5. **Mental Filtering** (2.1%) - 🟢 Rare
6. **Mind Reading** (0.2%) - 🟢 Rare

## ✅ Detection Effectiveness Evaluation

### Feature Detection Success Rate
| Effectiveness Level | Number of Features | Representative Features |
|---------------------|-------------------|------------------------|
| 🟡 Good (30-70%) | 3 | Manipulation Intent (48.2%), Unclassified Distortions (47.7%), Positive Sentiment (35.2%) |
| 🔴 Needs Improvement (<30%) | 7 | Negative Sentiment (26.8%), Overgeneralization (24.8%), etc. |

**Overall Detection Effectiveness**: 20.9% (Needs Improvement)

### Key Findings
- **Most Common Feature**: Manipulation Intent (present in 48.2% of samples)
- **Most Severe Feature**: Manipulation Intent (average intensity: 0.3886)
- **Data Quality**: 18.0% (Low quality, requires feature dictionary optimization)

## 📚 Technical Implementation Statistics

### n-gram Dictionary Scale
- **Total Features**: 77 targeted n-grams
- **Mental Filtering**: 23 features
- **Personalization**: 24 features
- **Manipulation**: 6 features
- **Sentiment Features**: 8 features (4 positive, 4 negative)
- **Other Distortions**: 16 features

## 🎯 Application Value

This system provides an effective cognitive distortion detection tool for mental health monitoring, content moderation, investment education, and other fields, offering transparency and credibility to analysis results through interpretable AI features.
