# 🚚 Vehicle Routing Simulation for Mid-Mile Distribution
Cost Optimization using Clarke–Wright Savings Algorithm
## 📌 Project Overview

This project focuses on analyzing and reducing transportation costs in mid-mile distribution using the Clarke–Wright Savings Algorithm, a well-known heuristic for solving the Vehicle Routing Problem (VRP).

The primary goal is to compare transportation cost without route optimization and with optimized vehicle routing, and to quantify how much cost is saved through efficient routing.

## 🎯 Objectives

Analyze transportation cost with and without vehicle routing

Minimize total travel distance

Improve route efficiency in mid-mile logistics

Quantify percentage cost savings

Demonstrate the effectiveness of the Clarke–Wright Savings Algorithm

## 🧠 Problem Description

The Vehicle Routing Problem (VRP) is a classic optimization problem in logistics and operations research.

It involves:

A central depot

Multiple delivery locations

A fleet of vehicles

The objective is to determine optimal routes such that:

Each location is visited exactly once

Vehicles start and end at the depot

Total distance and transportation cost are minimized

This problem is NP-hard, making heuristic approaches like Clarke–Wright highly practical for real-world scenarios.

## ⚙️ Algorithm Used
### 🔹 Clarke–Wright Savings Algorithm

The Clarke–Wright algorithm is a distance-based heuristic that builds efficient routes by calculating the savings achieved when combining two routes into one.

How it Works:

Start with one route per location (Depot → Location → Depot)

Calculate savings for combining two routes:

Savings(i, j) = d(Depot, i) + d(Depot, j) − d(i, j)


Sort savings in descending order

Merge routes with the highest savings while respecting constraints

Continue until no further improvements are possible

This approach significantly reduces redundant travel and overall cost.

## 💰 Cost Analysis & Results

Two routing scenarios were evaluated:

🔹 Scenario 1: Without Vehicle Routing (Baseline)

No optimization

Direct and independent trips

Higher total distance and fuel cost

Estimated Cost without Vehicle Routing:
₹225,466,437

🔹 Scenario 2: With Clarke–Wright Vehicle Routing

Optimized routes using savings-based merging

Reduced total distance

Better vehicle utilization

Estimated Cost with Vehicle Routing:
₹191,987,691

## 📉 Cost Savings Achieved
Metric	Value
Cost without Optimization	₹225,466,437
Cost with Optimization	₹191,987,691
Cost Savings	14.8%

👉 This clearly demonstrates that vehicle routing optimization can significantly reduce transportation costs in mid-mile logistics.

## 📊 Business Impact

14.8% reduction in transportation cost

Improved route efficiency

Reduced fuel consumption

Better logistics planning

Strong practical relevance for supply chain and distribution systems

## 🛠️ Tech Stack

Python

Jupyter Notebook

NumPy

Matplotlib

Optimization Logic (Clarke–Wright Savings Algorithm)


## 🔮 Future Enhancements

Add vehicle capacity constraints

Introduce time windows

Extend to multi-depot routing

Compare Clarke–Wright with metaheuristic algorithms

Integrate real-world map and traffic data

## 🏁 Conclusion

This project proves that applying the Clarke–Wright Savings Algorithm to mid-mile distribution can lead to significant cost savings and improved operational efficiency.
It highlights the importance of data-driven route optimization in modern logistics systems.
