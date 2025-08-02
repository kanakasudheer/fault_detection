 Power System Fault Detection and Classification using Machine Learning

This project presents a machine learning-based solution to detect, classify, and forecast power load behavior in an electrical power distribution system using phasor measurement data.


 📌 Problem Statement

Design a machine learning model to detect and classify different types of faults in a power distribution system. The model should distinguish between normal operation and fault conditions such as:

* Line-to-Ground (LG)
* Line-to-Line (LL)
* Double Line-to-Ground (LLG)
* Three-Phase Fault (LLL)

Additionally, the system forecasts future power load, helping to prevent faults through proactive load balancing.

💡 Proposed Solution

* Use supervised ML models trained on voltage and current phasors (from PMUs or simulation tools like MATLAB Simulink/PSCAD).
* Perform two-stage classification:

  * Stage 1: Fault vs Normal (Binary Classification)
  * Stage 2: LG / LL / LLG / LLL (Multi-class Classification)
* Predict future power load using an LSTM model for preventive maintenance and system reliability.


 🧠 Algorithm

### Fault Classification Pipeline:

1. *Data Collection*: Voltage and current phasor values
2. *Feature Extraction*:

   * Time-domain: RMS, peak, zero-crossing
   * Frequency-domain: FFT, harmonics
   * Sequence components (positive, negative, zero)
3. *Binary Classification*: Detect if fault exists
4. *Multi-Class Classification*: Classify fault type
5. *Model Evaluation*: Accuracy, F1-score, confusion matrix

 Power Load Prediction:

* Forecast future power consumption using time-series models (LSTM recommended)
🔭 Future Scope

* Real-time streaming with Apache Kafka or MQTT
* Fault localization and severity estimation
* Edge deployment for low-latency fault mitigation
* Renewable energy-aware forecasting
* Federated learning for privacy and scalability



✅ Conclusion

This project demonstrates the use of machine learning to intelligently:

* Detect and classify faults in power systems
* Forecast power load for proactive grid management

The system improves fault response time, enhances grid stability, and supports preventive maintenance.

\
