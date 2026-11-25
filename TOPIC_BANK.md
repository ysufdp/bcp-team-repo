# Topic Bank

## Lab 1: Paradigm Scan & Setup
* Status: Initial repository and file structure initialized. 
* Note: Thesis ideas and paradigm evaluations will be added following upcoming weekly lab sessions and lectures.

# Topic 1

## Travel Time Prediction and Multimodal Route Recommendation in Calamba, Laguna Using Gradient Boosting on Crowdsourced and Open Data: A Comparative Evaluation with Baseline Models
* Collect and preprocess crowdsourced GPS trips and open data for selected Calamba corridors.
* Train and compare LightGBM, Random Forest, Linear Regression, and a historical-average baseline.
* Evaluate with MAE, RMSE, and MAPE, using a chronological train/test split, with separate results for peak, off-peak, and rainy conditions.
* Develop a route recommender (Dijkstra/A*) that suggests multimodal routes ranked by time, fare, and transfers.
* Assess usability with commuters (for example, a SUS questionnaire with 20 to 30 respondents).

# Topic 2

## Vision-Based Adaptive Traffic Signal Control for a Mixed-Traffic Intersection in Calamba, Laguna: Comparing YOLO-Based Actuated Control with Fixed-Time Control Using Simulation
* Collect and annotate video frames from a selected Calamba intersection, covering peak, off-peak, night, and rainy conditions.
* Fine-tune and compare YOLO variants (for example, nano vs. small) on detection accuracy (mAP, precision, recall) and speed (FPS).
* Develop a queue-counting module using a virtual zone behind the stop line, and measure counting error (MAE) against manual counts.
* Implement a threshold-based actuated controller with minimum green, maximum green, yellow, and fail-safe fallback to fixed-time.
* Evaluate in SUMO against fixed-time control using average waiting time, queue length, and throughput under light, moderate, and heavy traffic.
* Build a small prototype (LEDs driven by an Arduino or ESP32) to demonstrate the logic.

# Topic 3

## Municipal Waste Collection Scheduling Using Greedy Allocation Algorithms and Machine Learning Demand Forecasting

* Forecast District Waste Demand Accurately: Build and train a supervised machine learning regression model (such as Random Forest or Gradient Boosting) using temporal, weather, and historical volume features to predict district-level waste generation with low error (measured via MAE and RMSE).
* Generate Capacity-Aware Pickup Schedules: Implement a greedy allocation algorithm that ranks collection zones by predicted demand, overflow urgency, and estimated service/travel effort, assigning pickups to available trucks without exceeding load or shift constraints.
* Reduce Uncollected & Overflowing Waste: Demonstrate through simulation experiments that the ML-and-greedy scheduling workflow leaves less uncollected or overflowing waste in high-demand zones compared to a static, fixed-interval baseline schedule.
* Maintain Fast Scheduling Execution & Low Overhead: Ensure the forecasting and greedy scheduling pipeline runs quickly on standard hardware (e.g., sub-second to a few seconds per schedule generation) using clean, modular Python code and lightweight data storage.
* Provide an Interactive Schedule & Metric View: Develop a simple, functional software interface (web dashboard or desktop/CLI tool) that lets users input or update fleet/zone parameters, generate schedules on demand, and inspect side-by-side comparisons of baseline versus greedy allocation metrics.

# Topic 4

## Enhancing Technical Indicator-Based Trading Signals with News and Announcement Sentiment: A Comparative Evaluation of Machine Learning Models on Selected Stocks

* Collect and align historical price data with timestamped news and announcements.
* Implement technical indicators and baseline rule-based signals.
* Apply FinBERT to produce sentiment and event features.
* Train and compare LightGBM, Random Forest, Logistic Regression, and LSTM using walk-forward validation.
* Evaluate predictions and backtest results against indicator-only and buy-and-hold baselines.
* Build a dashboard that shows signals with explanations and a clear "not financial advice" notice.
