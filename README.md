This project is a Deadlock Detection System implemented in Python using Resource Allocation Graphs (RAGs). It provides a Graphical User Interface (GUI) for users to add process-resource dependencies, detect deadlocks, and reset the system. The system uses NetworkX for graph management and cycle detection, and Tkinter for the GUI.

Features

1. Add processes and resources dynamically.
2. Allocate resources to processes using a directed graph.
3. Detect deadlocks using cycle detection in NetworkX.
4. Reset system to clear all dependencies.
5. User-friendly GUI built with Tkinter.

How It Works

Processes (P1, P2, etc.) and Resources (R1, R2, etc.) are represented as nodes in a Resource Allocation Graph (RAG).

If a process requests a resource, an edge is added (e.g., P1 → R1).

If a resource is assigned to a process, an edge is added (e.g., R1 → P2).

Cycle Detection Algorithm checks if there is a circular dependency (e.g., P1 → R1 → P2 → R2 → P1).

If a cycle exists, a deadlock warning is displayed. Otherwise, the system confirms no deadlocks detected
