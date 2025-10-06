# DetectPark

## Parkinson's Disease Detection from Voice Samples

### Final Year Project @ESME

DetectPark is a project that aims to detect Parkinson's disease through voice analysis. This project implements three different approaches to classify voice samples from healthy controls (HC) and Parkinson's disease (PD) patients using advanced signal processing, machine learning, and deep learning techniques.

## Getting Started

### Prerequisites

- **Python** : 3.11+ supported
- **Jupyter Notebook**

### Required Libraries

```bash
pip install librosa numpy pandas matplotlib seaborn scikit-learn tensorflow keras
```

### Usage

1. **Clone the repository** :

   ```bash
   git clone https://github.com/siyamr/detectpark.git
   cd detectpark/ParkinsonVoices
   ```

2. **Choose your approach** :
   - Open `ApprocheML.ipynb` for machine learning approach
   - Open `ApprocheDL.ipynb` for deep learning approach  
   - Open `ApprocheSignal.ipynb` for signal processing approach

3. **Run the notebooks** :
   - Execute cells sequentially to train and evaluate models
   - Each notebook is self-contained with data loading and preprocessing

## Dataset

The voice samples (sustained vowel /a/) used in this project are sourced from the research paper :
**"A Comprehensive Database of Parkinson's Disease Voice Recordings"** - [Nature](https://www.nature.com/articles/s41598-023-47568-w)

The dataset includes:

- **HC_AH/** : Healthy Control voice samples
- **PD_AH/** : Parkinson's Disease voice samples
- **Demographics_age_sex.xlsx** : Patient demographic information and extracted features

## Project Objectives

This project explores three distinct approaches for Parkinson's disease detection :

### 1. Machine Learning Approach (`ApprocheML.ipynb`)

- **Features** : LPC, LAR, Cepstral coefficients, MFCC, Parselmouth features
- **Methods** : Traditional ML algorithms (SVM, Random Forest, etc..)
- **Focus** : Feature engineering and statistical analysis

### 2. Deep Learning Approach (`ApprocheDL.ipynb`)

- **Features** : Mel-spectrograms and raw audio processing
- **Methods** : CNNs models
- **Focus** : Automatic feature extraction from spectrograms

### 3. Signal Processing Approach (`ApprocheSignal.ipynb`)

- **Features** : Raw audio signals and time-domain analysis
- **Methods** : Direct signal processing techniques
- **Focus** : Time-series analysis and signal characteristics

## Project Structure

```text
detectpark/
├── README.md
└── ParkinsonVoices/
    ├── ApprocheDL.ipynb          # Deep Learning approach
    ├── ApprocheML.ipynb          # Machine Learning approach
    ├── ApprocheSignal.ipynb      # Signal Processing approach
    ├── combined_df1.csv          # Processed features dataset 1
    ├── combined_df2.csv          # Processed features dataset 2
    ├── Demographics_age_sex.xlsx # Patient demographics and features
    ├── HC_AH/                    # Healthy Control voice samples
    │   ├── AH_064F_*.wav
    │   └── ...
    └── PD_AH/                    # Parkinson's Disease voice samples
        ├── AH_001F_*.wav
        └── ...
```

## Features

- **Multi-modal Analysis** : Three complementary approaches for robust detection
- **Feature Extraction** : Advanced audio feature engineering (MFCC, LPC, LAR, Cepstral)
- **Visualization** : Comprehensive data visualization and model performance analysis
- **Reproducible Results** : Structured notebooks with clear methodology

## Research Applications

This project contributes to :

- **Early Diagnosis** : Non-invasive Parkinson's detection through voice analysis
- **Comparative Study** : Evaluation of different ML/DL approaches
- **Medical AI** : Application of AI in healthcare diagnostics

## Contributors

- **Siyam R.** - ESME 2025 - AI Software Engineer
- **Léo C.** - ESME 2025

## License

This final year project is part of an academic research initiative at ESME Sudria.

---

**Note** : This project is for educational purposes only.
