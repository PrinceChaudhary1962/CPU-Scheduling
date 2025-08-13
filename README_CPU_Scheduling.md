# ⚙️ CPU Scheduling Algorithms in Python

This project simulates multiple **CPU scheduling algorithms** (FCFS, SJF, Priority, and Round Robin) to analyze process execution order, turnaround time, and waiting time. It helps visualize and compare scheduling strategies for better understanding of operating system process management.

---

## 📌 Problem Statement

In operating systems, CPU scheduling determines the order in which processes are executed by the CPU. The choice of scheduling algorithm impacts CPU utilization, throughput, turnaround time, and waiting time.

This project aims to:
- **Implement** different CPU scheduling algorithms.
- **Calculate** key performance metrics like waiting time & turnaround time.
- **Compare** algorithm efficiency with different process sets.
- **Visualize** Gantt charts for process execution order.

---

## 📊 Data Source

Input data consists of:
- **Process ID**
- **Arrival Time** (when the process arrives in the ready queue)
- **Burst Time** (CPU time required for execution)
- **Priority** (for priority scheduling)

Data can be entered manually or provided as a CSV/array inside the notebook.

---

## 🧠 Algorithms Implemented

### 🔷 First Come First Serve (FCFS)
- Non-preemptive
- Processes executed in the order of arrival
- Simple but can lead to **convoy effect**

### 🔷 Shortest Job First (SJF)
- Both **Non-preemptive** and **Preemptive (SRTF)** versions implemented
- Executes the process with the smallest burst time first
- Minimizes average waiting time but can cause starvation

### 🔷 Priority Scheduling
- **Non-preemptive** and **Preemptive** versions
- Higher priority processes executed first
- Can cause low-priority starvation

### 🔷 Round Robin (RR)
- Preemptive with fixed **time quantum**
- Fair scheduling for all processes
- Higher context switching overhead if quantum is too small

---

## ⚙️ Workflow

1. **Input processes** with arrival time, burst time, and priority (if applicable).
2. **Select algorithm** (FCFS, SJF, Priority, or RR).
3. **Simulate scheduling** to determine execution order.
4. **Calculate**:
   - Waiting Time (WT)
   - Turnaround Time (TAT)
   - Average WT & TAT
5. **Generate Gantt Chart** for visualization.
6. **Compare results** for different algorithms.

---

## 📈 Evaluation & Visualization

- **Gantt Chart** showing process execution timeline.
- **Tabular comparison** of waiting and turnaround times.
- **Performance metrics** for decision-making in OS scheduling.

**Example Output:**
```text
Process   AT   BT   CT   TAT   WT
P1        0    5    5    5     0
P2        1    3    8    7     4
P3        2    8   16   14     6

Average TAT: 8.67
Average WT: 3.33
```

**Visualization Example:**
Gantt chart showing time slots with process IDs.

---

## 📁 Project Structure
```
CPU-Scheduling/
├── CPU_Scheduling.ipynb
├── sample_input.csv
├── README.md
├── requirements.txt
└── .gitignore
```

---

## 📦 Requirements
- Python 3.x
- Pandas
- Matplotlib
- NumPy

Install dependencies:
```bash
pip install -r requirements.txt
```

---

## 🚀 How to Run
1. Open `CPU_Scheduling.ipynb` in Jupyter Notebook.
2. Provide process details in the input section or load from CSV.
3. Choose the scheduling algorithm to simulate.
4. Run all cells to view:
   - Process execution order
   - Performance metrics
   - Gantt chart visualization
