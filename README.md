# Real-Time QoS Optimization for Live Video Game Streaming

This project implements a **Real-Time Quality of Service (QoS) Optimization System** for live video game streaming platforms like **Twitch** and **YouTube Gaming**. It leverages:

* **Deep Neural Networks (DNN)** to predict user satisfaction based on network metrics.
* **BERT-based Sentiment Analysis** to interpret live chat sentiment.
* **Dynamic QoS Management** to automatically adjust bandwidth and latency.

---

## **Features**

* **Real-time monitoring:** Continuously evaluates QoS metrics such as latency, bitrate, and packet loss.
* **Sentiment analysis:** Analyzes live chat for user feedback on stream quality.
* **Adaptive adjustments:** Automatically scales bandwidth and latency for optimal viewer experience.
* **Plug-and-play:** Ready to use with live data streams and chat inputs.

---

## **Usage**

To use the system, simply run the main loop with sample QoS metrics and chat data:

```python
# Example usage:
# Sample DataFrame for QoS metrics
qos_data = pd.DataFrame({
    'latency': [20, 30, 25, 40],
    'bitrate': [5000, 4500, 5200, 4800],
    'packet_loss': [0.1, 0.05, 0.07, 0.02]
})

# Sample chat messages
chat_data = [
    "This stream is amazing!",
    "Why is it lagging so much?",
    "The quality is really good today.",
    "Buffering again... not great."
]

# Run the main loop
main_loop(qos_data, chat_data)
```

---

## **Setup and Installation**

1. Clone the repository:

   ```bash
   git clone https://github.com/your-repo/Real_Time_QoS_Optimization.git
   cd Real_Time_QoS_Optimization
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the script:

   ```bash
   python Real_Time_QoS_Optimization.py
   ```

4. For the Jupyter Notebook version:

   ```bash
   jupyter notebook Real_Time_QoS_Optimization.ipynb
   ```

---

## **Examples**

You can find various usage examples for different network conditions in the **Examples** section of the notebook:

* High Latency and High Packet Loss
* Smooth Streaming with Positive Feedback
* Mixed Quality with Fluctuating Latency
* Low Bitrate and Latency
* E-Sports Quality Streaming

---

## **Modules Used**

* `torch`: For deep neural network implementation.
* `transformers`: For BERT-based sentiment analysis.
* `scikit-learn`: For data preprocessing.
* `pandas`: For structured data handling.
* `numpy`: For numerical operations.
