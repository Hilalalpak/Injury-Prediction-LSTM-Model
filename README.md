# Sports Injury Risk Analysis Project 🏃‍♂️

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)]()
[![PyTorch](https://img.shields.io/badge/PyTorch-Latest-red)]()
[![License](https://img.shields.io/badge/License-MIT-green)]()

## 📋 Project Overview

This project implements a comprehensive sports injury risk analysis system using machine learning techniques. The system analyzes athlete data to predict injury risks and provide actionable insights for injury prevention.

### 🎯 Key Features

- Individual athlete risk profiling
- Real-time injury risk prediction using LSTM networks
- Workload analysis and optimization
- Performance metric tracking
- Comprehensive statistical analysis

## 📊 Data Sources

The project utilizes three main datasets collected between May 2016 and April 2018:

1. **Metrics Dataset**: Contains hip mobility and groin squeeze measurements
2. **Workload Dataset**: Game-specific performance and exertion metrics
3. **Injuries Dataset**: Complete injury tracking system data

## 🛠 Technical Architecture

### Data Processing Pipeline
```python
- Data Integration
- Feature Engineering
- Time Series Preparation
- Model Training
- Risk Assessment
```

### Key Components

- **LSTM Model**: Deep learning model for risk prediction
- **Early Stopping**: Prevents overfitting during training
- **Individual Models**: Separate models for each athlete
- **Risk Scoring System**: Comprehensive risk assessment

## 📈 Features

- `workload_7d`: 7-day cumulative workload
- `acwr`: Acute:Chronic workload ratio
- `workload_change`: Daily workload change percentage
- `hip_trend`: Mobility metrics trends
- `groin_trend`: Strength metrics trends
- `injuries_30d`: 30-day injury history
- `overall_risk`: Combined risk score

## 🚀 Getting Started

### Prerequisites

```bash
- Python 3.8+
- PyTorch
- pandas
- numpy
- scikit-learn
```

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/sports-injury-analysis.git
cd sports-injury-analysis
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

### Usage

1. Data Preparation:
```python
python src/data_preparation.py --input_path /path/to/data
```

2. Model Training:
```python
python src/train_model.py --config config/model_config.yaml
```

3. Risk Prediction:
```python
python src/predict.py --athlete_id <ID>
```

## 📊 Results

The model demonstrates varying performance across different athletes:
- Strong predictive accuracy for athletes with consistent training patterns
- Higher deviation in predictions for athletes with irregular workload patterns
- Successfully identifies high-risk periods and workload-related risk factors

## 📝 Key Findings

1. Workload patterns significantly impact injury risk
2. Individual athlete responses vary considerably
3. Hip mobility shows positive correlation with injury prevention
4. Rest periods are crucial for risk management

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📜 License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## 👥 Authors

- Hilal Alpak

## 📫 Contact

For questions and feedback, please contact:
- [GitHub Issues](https://github.com/yourusername/sports-injury-analysis/issues)

## 🙏 Acknowledgments

- Thanks to all athletes who participated in the data collection
- Sports medicine professionals who provided domain expertise
- Research team members who contributed to the analysis

## 📚 Citation

If you use this project in your research, please cite:
```bibtex
@article{alpak2024sports,
  title={Sports Injury Risk Analysis Using Machine Learning},
  author={Alpak, Hilal},
  year={2024}
}
```
