# 🌍 Smart Travel Planner – Multi-City Optimizer

## 📌 Overview

The **Smart Travel Planner** is a web-based application designed to optimize travel itineraries across multiple cities based on constraints such as **budget, time, and user-defined profit (fun score)**.

The system demonstrates the practical application of **Greedy Algorithms** and **Dynamic Programming** to solve real-world optimization problems.

---

## 🎯 Objectives

* To design an intelligent trip planner for multi-city travel
* To compare **Greedy vs Dynamic Programming** approaches
* To maximize **profit (fun score)** while minimizing **time and cost**
* To provide a clean and interactive user interface

---

## 🧠 Core Algorithms Used

### 🔹 Greedy Algorithm

* Selects the next city based on:

  `fun_score / (travel_cost + travel_time)`

* Provides a **fast but approximate solution**

* Works by making **locally optimal choices**

---

### 🔹 Dynamic Programming (DP)

* Uses a **Knapsack-based approach**

* Maximizes total profit under:

  * Budget constraint
  * Time constraint

* Provides a **globally optimal solution**

* Considers all possible combinations efficiently

---

## ⚙️ Features

### 🟢 Input Features

* Supports up to **10 cities**
* User-defined:

  * City names
  * Travel cost matrix
  * Travel time matrix
  * Fun score (profit) per city
  * Total budget
  * Total available time

---

### 🟢 Optimization Features

* Generates:

  * **Greedy-based itinerary**
  * **DP-based optimal itinerary**

* Displays:

  * Selected cities / route
  * Total cost
  * Total time
  * Total profit

---

### 🟢 Comparison Feature

* Side-by-side comparison of:

  * Greedy vs DP results

* Highlights:

  * Speed vs Accuracy trade-off
  * Local vs Global optimization

---

### 🟢 UI/UX Features

* Clean and modern interface
* Responsive design
* Interactive input forms
* Visual result display
* Easy-to-use layout

---

### 🟢 Advanced Features

* Constraint-based optimization (time + budget)
* Real-time computation
* Scalable up to 10 cities
* Modular architecture (C++ + Node.js)

---

## 🏗️ Project Structure

```
CCC/
│
├── src/
│   ├── main.cpp        # Entry point
│   ├── dp.cpp          # Dynamic Programming logic
│   ├── greedy.cpp      # Greedy algorithm logic
│   ├── dp.hpp
│   ├── greedy.hpp
│
├── public/             # Frontend files
├── server.js           # Node.js backend
├── package.json
├── optimizer.exe       # Compiled C++ executable
```

---

## 🔄 System Workflow

1. User enters travel data in the web interface
2. Frontend sends request to backend
3. Backend executes C++ optimizer
4. Algorithms process the input
5. Results are returned and displayed

---

## 💻 Technologies Used

* **Frontend:** HTML, CSS, JavaScript
* **Backend:** Node.js
* **Core Logic:** C++
* **Integration:** Child Process Execution

---

## 🚀 How to Run the Project

### Step 1: Install Dependencies

```
npm install
```

---

### Step 2: Compile C++ Code

```
g++ src/main.cpp src/dp.cpp src/greedy.cpp -o optimizer
```

---

### Step 3: Start Server

```
node server.js
```

---

### Step 4: Open in Browser

```
http://localhost:3000
```

---

## 📊 Performance

| Algorithm | Time Complexity | Nature      |
| --------- | --------------- | ----------- |
| Greedy    | O(n log n)      | Approximate |
| DP        | O(n × budget)   | Optimal     |

---

## 🧪 Sample Input

* Cities: A, B, C, D
* Budget: 100
* Time: 10 units
* Fun Scores: [10, 20, 30, 25]

---

## 📈 Sample Output

* **Greedy Result:**

  * Cities: A → C → D
  * Profit: 55

* **DP Result:**

  * Cities: B → C → D
  * Profit: 75

---

## 🎤 Key Learning Outcomes

* Understanding of optimization problems
* Practical implementation of Greedy & DP
* Trade-off between speed and optimality
* Real-world application of algorithms

---

## 🧬 Real-World Applications

* Travel planning systems
* Logistics optimization
* Resource allocation problems
* Budget management tools

---

## 📸 Screenshots

<img width="1909" height="954" alt="image" src="https://github.com/user-attachments/assets/fb6ed701-592b-49ba-9e96-9330467955b6" />
<img width="1909" height="954" alt="image" src="https://github.com/user-attachments/assets/4c33c275-56e8-43b5-a9f9-31eeed3099b5" />
<img width="906" height="817" alt="image" src="https://github.com/user-attachments/assets/7691116e-6a83-43a5-9d3b-9ae458f4f0bf" />
<img width="906" height="817" alt="image" src="https://github.com/user-attachments/assets/e42883e6-f5f3-4b07-9fba-e9c9e64371e9" />
<img width="1915" height="954" alt="image" src="https://github.com/user-attachments/assets/6620ab40-78f0-4853-9a52-85daac121f57" />


## 🏁 Conclusion

This project successfully demonstrates how classical algorithms like **Greedy** and **Dynamic Programming** can be applied to solve real-world problems efficiently.

It highlights the importance of choosing the right algorithm based on constraints such as **time, accuracy, and scalability**.
