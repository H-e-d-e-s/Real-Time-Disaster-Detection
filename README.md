# Real-Time Disaster Detection from Social Media

Our BERT-powered classifier achieved an impressive **82% accuracy** in distinguishing real disaster tweets from regular social media noise.

## The Science Behind the Magic

### The Dataset Journey
- **Data Source**: Curated collection of Twitter messages labeled as either disaster-related (1) or normal tweets (0)
- **Scale**: Over 15,000 tweets for training, plus additional test data
- **Challenge**: Highly imbalanced dataset (71.6% normal vs 28.4% disaster tweets)

### Our AI Arsenal

#### **BERT-Powered Classification**
- **Model**: Fine-tuned BERT-base-uncased transformer
- **Architecture**: Custom classifier with dropout regularization
- **Training**: 25 epochs with AdamW optimizer
- **Performance**: Achieved 82% accuracy with strong precision (87.3%)

#### **Topic Discovery**
- **Tool**: BERTopic for unsupervised topic modeling
- **Purpose**: Understanding what people actually talk about during disasters
- **Insight**: Revealed distinct conversation patterns between emergency and normal situations

#### **Geographic Intelligence**
- **Technology**: spaCy Named Entity Recognition
- **Feature**: Automatic location extraction from tweets
- **Visualization**: Interactive maps showing disaster hotspots
- **Application**: Could help emergency responders prioritize areas

## Visual Intelligence

Our system doesn't just classify - it tells a story through data:

- **Word Clouds**: Showing the vocabulary of disaster vs normal tweets
- **Topic Visualizations**: Interactive charts revealing conversation themes  
- **Training Curves**: Real-time monitoring of model learning
- **Geographic Maps**: Pinpointing disaster locations on interactive maps
- **Confusion Matrices**: Understanding where our model excels and struggles

## Performance Deep Dive

| Metric | Score | What This Means |
|--------|-------|-----------------|
| **Accuracy** | 82.0% | 4 out of 5 tweets correctly classified |
| **Precision** | 87.3% | When we say "disaster", we're right 87% of the time |
| **Recall** | 69.3% | We catch about 70% of actual disaster tweets |
| **F1-Score** | 77.2% | Balanced measure of precision and recall |


### Quick Start
1. **Data Preparation**: Load and merge tweet datasets
2. **Text Preprocessing**: Clean tweets, remove URLs, normalize text
3. **Model Training**: Fine-tune BERT on our disaster detection task
4. **Evaluation**: Test performance on unseen data
5. **Visualization**: Generate insights and maps

## Key Insights Discovered

### Language Patterns
- **Disaster tweets** tend to use urgent language: "help", "emergency", "collapsed", "flooding"
- **Normal tweets** focus on daily life: "work", "coffee", "weekend", "friends"

### Geographic Patterns  
- Extracted location mentions reveal disaster-prone areas
- Could enable real-time geographic risk assessment

### Temporal Patterns
- Training curves show model learning stabilizes around epoch 15-20
- Early stopping could prevent overfitting


## Performance Notes

- **GPU Recommended**: Training takes ~2 hours on GPU vs 12+ hours on CPU
- **Memory**: Requires ~8GB RAM for comfortable operation
- **Storage**: Model files total ~850MB

## Achievements

- Successfully classified disaster tweets with 82% accuracy
- Implemented end-to-end pipeline from raw data to insights
- Created interactive visualizations for data exploration
- Integrated geographic analysis for spatial intelligence
- Built comprehensive evaluation framework

---