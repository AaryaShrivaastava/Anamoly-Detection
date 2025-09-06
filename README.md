# 🔍 Real-Time Anomaly Detection System

A web-based application for detecting anomalies in web server logs using unsupervised machine learning algorithms.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-1.0.0-green.svg)
![ML](https://img.shields.io/badge/ML-Unsupervised-orange.svg)

## 📋 Project Overview

This project implements a real-time anomaly detection system that monitors web server logs and identifies unusual patterns using various unsupervised machine learning techniques. It's designed to help developers and system administrators detect potential security threats, performance issues, and abnormal user behavior.

## ✨ Features

### Core Functionality
- **Real-time Log Processing**: Simulates and processes web server logs in real-time
- **Multiple Detection Algorithms**:
  - Isolation Forest
  - DBSCAN (Density-Based Spatial Clustering)
  - Local Outlier Factor (LOF)
  - Statistical Methods
- **Interactive Visualization**: Live charts showing anomaly trends
- **Customizable Parameters**: Adjust detection sensitivity and log generation rates
- **Performance Metrics**: Real-time display of precision, recall, F1 score, and accuracy

### Objectives Covered

1. **Log Ingestion and Preprocessing** ✅
   - Simulates Apache/Nginx access logs
   - Extracts features like response time, status codes, IP addresses
   - Real-time data streaming

2. **Unsupervised Model Training** ✅
   - Implements Isolation Forest for anomaly detection
   - DBSCAN for density-based clustering
   - Statistical methods for outlier detection

3. **Persistence and Notification** ✅
   - Stores anomaly events in browser memory
   - Visual alerts for detected anomalies
   - Real-time notification system

4. **API Integration** ✅
   - User-friendly web interface
   - RESTful-like data handling
   - Real-time data streaming

5. **Modern Web Development** ✅
   - Responsive design
   - Real-time visualizations with Chart.js
   - Interactive controls

6. **Feature Engineering** ✅
   - Response time analysis
   - Request rate monitoring
   - Error pattern detection
   - Traffic pattern analysis

## 🚀 Quick Start

### Deploy on Vercel

1. Click the button below to deploy:

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/yourusername/realtime-anomaly-detection)

2. Or deploy manually:
```bash
npm i -g vercel
vercel
```

### Local Development

1. Clone the repository:
```bash
git clone https://github.com/yourusername/realtime-anomaly-detection.git
cd realtime-anomaly-detection
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm start
```

4. Open your browser and navigate to:
```
http://localhost:3000
```

## 📁 Project Structure

```
realtime-anomaly-detection/
│
├── index.html           # Main application file
├── package.json         # Project configuration
├── README.md           # Documentation (this file)
├── vercel.json         # Vercel deployment config
└── .gitignore          # Git ignore file
```

## 🎮 How to Use

1. **Select Algorithm**: Choose from Isolation Forest, DBSCAN, LOF, or Statistical methods
2. **Adjust Threshold**: Set the sensitivity for anomaly detection (0.01 - 0.20)
3. **Configure Log Rate**: Control how fast logs are generated (100ms - 5000ms)
4. **Set Anomaly Rate**: Simulate the percentage of anomalous logs (0% - 30%)
5. **Start Detection**: Click the "Start Detection" button to begin monitoring
6. **Monitor Results**: Watch real-time logs, statistics, and visualizations

## 🔧 Configuration

### Algorithm Parameters

| Algorithm | Description | Best For |
|-----------|-------------|----------|
| Isolation Forest | Isolates anomalies using random partitioning | High-dimensional data, fast detection |
| DBSCAN | Density-based clustering | Spatial anomalies, varying densities |
| Local Outlier Factor | Measures local density deviation | Local anomalies, complex patterns |
| Statistical | Z-score and IQR methods | Simple anomalies, baseline detection |

### Threshold Settings

- **Low (0.01-0.05)**: High sensitivity, more anomalies detected
- **Medium (0.05-0.15)**: Balanced detection
- **High (0.15-0.20)**: Low sensitivity, only severe anomalies

## 📊 Features Extracted

The system analyzes multiple features from web server logs:

1. **Response Time Distribution**: Identifies unusually slow or fast responses
2. **Request Rate Patterns**: Detects traffic spikes or drops
3. **HTTP Status Codes**: Monitors error rate patterns
4. **User Agent Analysis**: Identifies bot traffic or suspicious agents
5. **Geographic Distribution**: Detects requests from unusual locations
6. **Request Size**: Flags abnormally large or small requests
7. **Session Duration**: Identifies outlier session behaviors
8. **API Endpoint Usage**: Monitors unusual endpoint access patterns

## 🎯 Use Cases

- **Security Monitoring**: Detect potential DDoS attacks, brute force attempts
- **Performance Analysis**: Identify slow queries, resource bottlenecks
- **User Behavior Analysis**: Find unusual user patterns, bot detection
- **System Health Monitoring**: Detect service degradation, error spikes
- **Compliance Monitoring**: Track and alert on policy violations

## 🧪 Testing

The application includes simulated log generation for testing:

1. Adjust the **Anomaly Rate** slider to control the percentage of anomalous logs
2. Use different **algorithms** to compare detection effectiveness
3. Modify the **threshold** to balance between false positives and false negatives
4. Monitor the **performance metrics** to evaluate accuracy

## 📈 Performance Metrics

The system displays real-time performance metrics:

- **Precision**: Ratio of true anomalies to all detected anomalies
- **Recall**: Ratio of detected anomalies to all actual anomalies
- **F1 Score**: Harmonic mean of precision and recall
- **Accuracy**: Overall correctness of the detection

## 🔄 Future Enhancements

- [ ] Add data export functionality (CSV, JSON)
- [ ] Implement real log file upload and processing
- [ ] Add more ML algorithms (One-Class SVM, Autoencoders)
- [ ] Include time-series analysis
- [ ] Add email/webhook notifications
- [ ] Implement data persistence with IndexedDB
- [ ] Add multi-user support with authentication
- [ ] Create REST API for external integrations

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- Chart.js for visualization
- Inspiration from real-world log monitoring systems
- Community contributions and feedback

## 📧 Contact

For questions or support, please open an issue on GitHub or contact the maintainers.

---

**Made with ❤️ for the DevOps and Security Community**