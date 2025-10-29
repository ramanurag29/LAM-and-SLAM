# 🤖 Advanced Multi-Algorithm SLAM

### A research-driven exploration into how robots **perceive, localize, and learn**.

When I first began exploring SLAM, I wasn’t just interested in mapping environments — I wanted to understand *how robots build awareness from uncertainty*. This project became a complete learning curve, where theory met debugging, and equations slowly turned into working systems.

The goal was simple in definition yet complex in execution:  
to benchmark multiple localization algorithms under identical conditions and see how each handles real-world uncertainty.  
I implemented six approaches — from **Dead-Reckoning**, the simplest form of odometry integration, to **GraphSLAM**, which globally optimizes pose estimates using constraints. In between came the filters that shaped modern robotics: **EKF**, **UKF**, **Neural-Net**, and **QPSO**.

Each step exposed a new challenge:
- Early on, my robot’s trajectory drifted uncontrollably — a reminder that “good equations” don’t guarantee *good estimation*.
- Tuning covariance matrices felt more like art than math.  
- Neural networks overfitted quickly; learning bias correction required careful data curation.  
- QPSO’s swarm-based optimization ran beautifully in theory but demanded significant runtime balancing.

Through these iterations, I learned to think in both directions: from **physical motion** (how sensors perceive) and from **mathematical abstraction** (how uncertainty propagates).  
Once all six algorithms stabilized, I compared them across metrics like **RMSE**, **time complexity**, and **robustness to noise**. GraphSLAM stood out — reducing localization error by nearly 97% compared to the baseline.

What started as a coding experiment evolved into a genuine systems-engineering insight:  
robust localization isn’t about one perfect algorithm; it’s about the *right blend* of models, learning, and feedback.

This repository represents that journey — from instability to precision, from isolated math to cohesive motion.  
All 950+ lines of MATLAB here aren’t just code; they’re the reflection of an evolving understanding of how autonomous systems **see, learn, and decide**.

---

*“Every time the robot got lost, I learned something new about control, noise, and trust in uncertainty.”*
