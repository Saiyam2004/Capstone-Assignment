Delivery Route Optimization 

This project solves a simplified delivery route optimization problem for an e-commerce company using multiple algorithmic strategies taught in the Design & Analysis of Algorithms course.

The goal is to plan delivery routes starting from a Warehouse, visiting customers C1, C2, C3, selecting parcels based on value, respecting time windows, and finding the shortest possible route.

🚀 Features Implemented
✔ 1. Input Modeling

City represented as nodes

Distances stored in a distance matrix

Parcels have value, weight, and time windows

Vehicle has capacity 30

✔ 2. Greedy Algorithm (Parcel Selection)

Uses value / weight ratio

Selects parcels that give highest profit within capacity

Simple and fast (O(n log n))

✔ 3. Time-Window Feasibility Checker

Ensures delivery to each customer happens between:

Earliest time

Latest time

Includes waiting if the vehicle reaches early

✔ 4. TSP (Brute Force)

Tests all possible visiting orders of customers

Finds the shortest route returning to the warehouse

Works because problem size is small (3 customers)

✔ 5. Graph Algorithms
Dijkstra

Computes shortest path from the warehouse to all customers

Prim’s MST

Connects all customers in minimum total distance

Useful when the vehicle doesn’t need to return to warehouse

✔ 6. Graph Visualization

Using networkx + matplotlib:

City graph with distances

Highlighted TSP route
