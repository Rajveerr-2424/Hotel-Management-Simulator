# README

🏨 HOTEL MANAGEMENT SIMULATOR
A full-stack web application that simulates hotel room management and booking optimization using Greedy and Knapsack algorithms to maximize hotel revenue and optimize resource utilization.

🚀 OVERVIEW
The Hotel Management Simulator allows users to input guest booking requests, run algorithmic simulations, and analyze results through data visualization and reports.
It demonstrates how algorithmic decision-making (specifically Greedy and Knapsack approaches) can be applied to real-world hotel management for better profit optimization and resource allocation.

🧠 CORE CONCEPT
Every booking consumes a certain number of room-nights (rooms × stay duration).
The hotel has a fixed capacity of room-nights.
The system decides which guests to accept to maximize total profit.

Two algorithms are used:

Greedy Algorithm (Profit-to-Room-Night Ratio):

Sort guest requests by (Payment / Room-Night) ratio in descending order.

Accept guests until capacity is reached.

Fast but approximate.

0/1 Knapsack Algorithm:

Finds the optimal combination of guests to yield maximum total profit without exceeding capacity.

Slower but guarantees best results.

🧩 FEATURES

🎟️ Guest Booking Input

Input guest name, stay duration, payment offered, and rooms requested.

Built-in calculator for auto-calculating payment based on stay length and room type.

🏨 Simulation Controls

Set total available rooms and simulation days.

Choose algorithm: Greedy, Knapsack, or comparison mode.

📊 Results Dashboard

Accepted and rejected guest lists.

Occupancy rate percentage.

Total revenue for both algorithms.

Algorithm performance comparison.

📈 Data Visualization

Bar graph comparing revenue (Greedy vs Knapsack).

Pie chart showing occupancy/room usage.

Visualization toggle (ON/OFF).

🧾 Report Generation

Export results as professional PDFs (not CSV).

Include summary, guest lists, charts, and metrics using jsPDF or pdfmake.

⚙️ TECH STACK

Frontend: React.js + Tailwind CSS
Backend: Node.js (Express.js)
Database: SQLite
Visualization: Chart.js or Recharts
PDF Reports: jsPDF or pdfmake

Justifications:

Node.js for fast, event-driven backend suitable for real-time simulation.

SQLite for lightweight, file-based data storage ideal for prototypes and algorithm testing.

🧮 ALGORITHMIC FLOW

Input guest data.

Calculate total room-night capacity.

Run selected algorithm (Greedy or Knapsack).

Compute accepted bookings.

Calculate total revenue and occupancy rate.

Display comparison dashboard and generate report.

🧠 LEARNING MODE (Optional)
A toggle mode that visually explains each algorithm step-by-step, showing which bookings are accepted or skipped — useful for educational demonstrations.

📄 INSTALLATION & SETUP

Clone the repository:
git clone https://github.com/Rajveerr-2424/Hotel-Management-Simulator.git

cd hotel-management-simulator

Install dependencies:
npm install

Run backend:
npm run server

Run frontend:
npm start

📊 EXAMPLE OUTPUT

Guest | Rooms | Days | Payment | Algorithm | Status
Alice | 2 | 3 | ₹9000 | Greedy | Accepted
Bob | 1 | 5 | ₹7000 | Greedy | Rejected

Total Revenue (Greedy): ₹9000
Total Revenue (Knapsack): ₹10,500
Occupancy Rate: 82%

🧰 FUTURE ENHANCEMENTS

Support for multiple hotels or branches.

Seasonal pricing logic.

Dynamic revenue optimization based on trends.

Live performance graphs for algorithms.

👨‍💻 AUTHORS
A6_B1_13 Rajveerr Awachat
A6_B3_37 Pranav Gandhi
and
A6_B1_16 Deepika Pampati

B.Tech CSE, Ramdeobaba University

🧾 LICENSE
This project is licensed under the MIT License — free for educational use only.
