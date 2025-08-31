# RASD

# Road Hazard Detection System – User Story Backlog

This document outlines the user stories, priorities, and acceptance criteria for the Road Hazard Detection System, covering pothole and speed bump detection under various conditions.

---

## 📌 User Story Backlog

| ID  | Title                           | User Story (IEEE Format)                                                                                                                                         | Priority | Acceptance Criteria                                                                                                                                                                                                 |
|-----|---------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| P1  | Pothole Detection – Morning     | As a driver commuting in the morning, I want the system to detect potholes ahead so that I can reduce speed smoothly.                                             | High     | • System detects potholes in clear conditions <br> • Driver is alerted early enough to reduce speed safely <br> • False positives are minimized <br> • Pothole is logged with GPS, time, and severity for reporting |
| P2  | Pothole Detection – Night       | As a driver traveling at night, I want the system to detect potholes in low visibility so that I can avoid sudden swerves.                                        | High     | • System functions reliably under low-light conditions <br> • LiDAR + camera fusion enables accurate detection <br> • Driver receives a timely alert <br> • Pothole is logged with GPS, time, and severity          |
| P3  | Pothole Detection – Extreme Wx  | As a driver in heavy rain, I want potholes detected despite water or dust so that I can prevent accidents.                                                        | Medium   | • Detection accuracy remains acceptable in rain/dust <br> • Alerts are delivered to the driver in real time <br> • Pothole is logged with GPS, time, and severity                                                    |
| S1  | Speed Bump Detection – Morning  | As a driver commuting in the morning, I want the system to detect speed bumps so that I can slow down safely.                                                     | High     | • System detects speed bumps under normal visibility <br> • Driver is prompted to reduce speed before crossing <br> • Alerts are consistent and reliable                                                             |
| S2  | Speed Bump Detection – Night    | As a driver at night, I want the system to recognize even unmarked bumps so that I am warned early.                                                               | High     | • System identifies both marked and unmarked bumps at night <br> • Driver receives a clear and timely warning <br> • Detection accuracy remains high                                                                 |
| S3  | Speed Bump Detection – Extreme Wx | As a driver in fog or storms, I want bumps detected or supplemented by previous logs so that I can ensure safety.                                                | Medium   | • System detects bumps despite reduced visibility <br> • False positives minimized <br> • Detection supplemented with historical data if visibility is too low <br> • Driver alerted in time to act safely          |

---

## ⚙️ Non-Functional Requirements (NFR)

- **Reliability**: 24/7 operation, minimal downtime  
- **Usability**: Alerts must be simple and non-distracting  
- **Scalability**: Can handle multiple anomalies in a single trip  
- **Maintainability**: Detection models are easy to update  

---

## 📊 Acceptance Criteria – Improvements

To make the requirements measurable and testable (aligned with IEEE standards):

- **Performance Constraints**:  
  - Alerts must be issued within **1 second**  
  - Logging must occur within **< 5 seconds** delay  

- **Accuracy Thresholds**:  
  - ≥ **90% detection rate** in normal conditions  
  - ≥ **80% detection rate** in fog or extreme weather  

- **Safety Considerations**:  
  - **No false negatives** for severe potholes  
  - Alerts must always provide sufficient reaction time  

---

## ✅ Summary

This backlog ensures that the system:  
- Works across **time (day/night)** and **environmental conditions (clear, fog, rain, dust)**  
- Provides **timely, accurate alerts** for driver safety  
- Maintains **reliability and scalability** for real-world road conditions  

