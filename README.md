# Industrial Engineering Projects

A collection of quantitative optimization and risk modeling projects applying operations research methods — linear programming, binary integer programming, and statistical inference — to logistics, fraud risk, and engineering design problems.

---

## Payment Fraud Optimization Engine
**Tools:** Python, PuLP, NumPy

Built a real-time transaction risk-decisioning framework on 590,000+ records, using an interpretable Logistic Regression model to score fraud probability per transaction with clear statistical inference — achieving a 72.6% reduction in data memory footprint to support low-latency scoring.

Formulated a Binary Integer Programming model to optimize approve/flag decisioning under a fixed review-capacity constraint (10 hours of manual review per day), preventing $17,248 in fraud losses over a 5-day window while operating within throughput limits.

Designed a real-time streaming simulation processing 118,534 transactions 
sequentially at 82 transactions/minute, dynamically ranking fraud risk scores 
to flag the top 3% for review while modeling review queue depth against analyst 
capacity constraints — demonstrating throughput-aware decisioning logic at scale.

*Note: Built and validated at 590,000+ record scale. The scoring and decisioning architecture 
is designed to generalize to higher-volume streaming contexts — in a production environment, 
the per-transaction logistic regression scoring function would integrate with a real-time 
stream processing layer (e.g., Kafka/Flink) with the BIP threshold optimization running on 
rolling capacity windows rather than daily batches.*

[View notebook](Payment_Fraud_Optimization_Engine.ipynb)

---

## Supply Chain Network Optimization Model
**Tools:** Python, PuLP, Pandas

Modeled a linear programming optimization engine across 500+ constraint variables to minimize transportation overhead and accelerate logistics velocity, projecting an 18% transportation cost reduction under baseline demand assumptions.

Includes a Python dashboard to stress-test optimization outputs against demand volatility and support capital investment decisions.

[View notebook](Supply_Chain_Optimization_Project.ipynb)

---

## Automated Spring Design Visualization Program
**Tools:** Python, MATLAB, NumPy

Programmed a high-performance filtering mask to isolate the top 18% of viable spring configurations within a 5% precision tolerance, using matrix array manipulations to calculate parameter limits and simulate design viability under input volatility.

[View notebook](Automated_Spring_Design_Program.ipynb)

---

## License
MIT
