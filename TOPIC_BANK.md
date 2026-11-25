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
