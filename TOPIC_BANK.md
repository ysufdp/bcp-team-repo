# Topic Bank: Team BCP

We add one entry after every lab (Labs 01 to 10) using the template from the Laboratory Module. Scores are team averages from 1 to 5. **Interest** is how much we want to spend a thesis term on the idea. **Feasibility** covers data access, compute, skills, and time (5 = easy).

## Shortlist

| Idea | Paradigm | Lab | Interest | Feasibility | Status |
| --- | --- | --- | --- | --- | --- |
| Calamba TransitPredict: travel time prediction and multimodal route recommendation | Classical machine learning, graph routing | 01 | 4 | 4 | Shortlisted (Week 1) |
| Calamba AdaptiveSignal: vision-based adaptive traffic signal control | Computer vision (YOLO), simulation | 01 | 4 | 3 | Shortlisted (Week 1) |
| Calamba WasteRoute: municipal waste collection scheduling with ML forecasting | Classical machine learning, greedy optimization | 01 | 5 | 4 | Shortlisted (Week 1) |
| SentimTrade: stock trading signals enhanced with news sentiment | NLP (FinBERT), time-series ML | 01 | 3 | 4 | Shortlisted (Week 1) |

---

## Lab 01: Paradigm scan (Week 1)

Four raw ideas from the paradigm tour. Breadth over polish.

### 1. Calamba TransitPredict: travel time prediction and multimodal route recommendation

- **Idea:** A predictive routing system that estimates travel times across Calamba corridors using Gradient Boosting and recommends multimodal routes ranked by time, fare, and transfers.
- **Problem it addresses:** Commuters in Calamba face unpredictable travel times during peak hours and rainy weather, with no unified tool balancing travel speed, fare cost, and jeepney/tricycle transfers.
- **Closest existing work:** Classical ML travel-time forecasting (LightGBM, Random Forest) paired with shortest-path graph algorithms (Dijkstra / A*) and System Usability Scale (SUS) commuter evaluation.
- **Data needed:** Crowdsourced GPS trip logs and open road/transit data for selected Calamba corridors, labeled by peak, off-peak, and rainy conditions.
- **Compute needed:** Laptop (Python, scikit-learn / LightGBM) for model training and routing simulation.
- **Biggest risk:** Collecting enough representative crowdsourced GPS trajectories across varied weather and peak conditions.
- **Team interest:** 4/5 · **Feasibility:** 4/5

### 2. Calamba AdaptiveSignal: vision-based adaptive traffic signal control

- **Idea:** A YOLO-based vehicle detection and virtual stop-line queue-counting system that dynamically adjusts traffic light green times in simulation, paired with a hardware LED prototype.
- **Problem it addresses:** Fixed-time traffic signals at mixed-traffic intersections in Calamba cause unnecessary delays and long queues when traffic volume fluctuates across peak, off-peak, night, and rainy periods.
- **Closest existing work:** Real-time object detection using YOLO variants combined with threshold-based actuated signal controllers evaluated in SUMO (Simulation of Urban MObility).
- **Data needed:** Annotated intersection video frames from a Calamba intersection covering peak, off-peak, night, and rainy conditions.
- **Compute needed:** Colab GPU for fine-tuning YOLO models; laptop for SUMO traffic simulation; Arduino or ESP32 with LEDs for the logic prototype.
- **Biggest risk:** Reduced vehicle detection accuracy during heavy rain or low-light night conditions, and securing clear intersection footage.
- **Team interest:** 4/5 · **Feasibility:** 3/5

### 3. Calamba WasteRoute: municipal waste collection scheduling with ML forecasting

- **Idea:** A software tool that predicts district-level waste generation using supervised regression (Random Forest / Gradient Boosting) and generates capacity-aware truck pickup schedules via a greedy allocation algorithm.
- **Problem it addresses:** Static, fixed-interval waste collection schedules fail to adapt to demand spikes, leaving high-demand zones in Calamba with uncollected or overflowing waste.
- **Closest existing work:** Demand-driven vehicle routing and greedy resource allocation paired with tabular regression models evaluated against fixed-interval baselines.
- **Data needed:** Historical district waste volume records, temporal calendars, weather data, and fleet capacity/zone parameters.
- **Compute needed:** Laptop (Python, scikit-learn) for forecasting, greedy scheduling simulation, and an interactive web/desktop dashboard.
- **Biggest risk:** Obtaining granular historical waste volume records per district from local municipal offices.
- **Team interest:** 5/5 · **Feasibility:** 4/5

### 4. SentimTrade: stock trading signals enhanced with news sentiment

- **Idea:** A quantitative trading signal dashboard that combines technical indicators with FinBERT financial news sentiment features across LightGBM, Random Forest, Logistic Regression, and LSTM models.
- **Problem it addresses:** Indicator-only trading rules react late to market-moving announcements and corporate news.
- **Closest existing work:** Financial sentiment analysis using FinBERT ([Araci, 2019](https://arxiv.org/abs/1908.10063)) combined with walk-forward backtesting against buy-and-hold and technical-indicator baselines.
- **Data needed:** Historical stock price series aligned with timestamped financial news and company announcements.
- **Compute needed:** Colab GPU for FinBERT inference and LSTM training; laptop for walk-forward backtesting and dashboard display.
- **Biggest risk:** Look-ahead bias in timestamp alignment and lower thesis novelty compared to localized community-impact problems.
- **Team interest:** 3/5 · **Feasibility:** 4/5
