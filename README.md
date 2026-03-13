# QState-Arena - Learning Quantum Gates
A mini project built as part of the **PESUIO** course at PES University, aiming to help understand and visualize quantum gates and qubits.

*A gamified, interactive 2-qubit quantum state simulator with Bloch sphere visualization.*

Quantum State Builder is an educational and interactive Python application that lets users create, manipulate, and measure 2-qubit quantum states using real quantum gates. It visualizes each qubit on a Bloch sphere, displays joint-state probabilities, and guides the player through multiple quantum challenges — including creating Bell states and phase-entangled states.

The project uses **Tkinter** for the GUI and **Qiskit** for quantum simulation, with **Matplotlib** for 3D Bloch sphere rendering and a custom “entanglement glow” effect.



## 🚀 **Features**

### 🎮 **Gameplay & Levels**

The game consists of **five progressive levels**:

1. Prepare `|00⟩`
2. Prepare `|11⟩`
3. Prepare the superposition `|++⟩`
4. Create a Bell state `|Φ⁺⟩ = (|00⟩ + |11⟩)/√2`
5. Create the phase-entangled state `( |01⟩ + i|10⟩ ) / √2`

Each level evaluates your state’s **fidelity** and awards points when successful.



### ⚛️ **Quantum Gate Controls**

You can apply common single-qubit and two-qubit gates:

| Gate | Description                                        |
| - | -- |
| X    | Bit flip                                           |
| Y    | Bit + phase flip                                   |
| Z    | Phase flip                                         |
| H    | Hadamard (superposition)                           |
| S    | Phase π/2                                          |
| T    | Phase π/4                                          |
| CX   | Controlled-NOT (custom control & target selection) |



### 📊 **Real-Time Visualization**

The interface includes:

* **Two Bloch spheres** (one per qubit)
* **Glow effect** that intensifies as the qubits become mixed/entangled
* **Joint state probability bar chart**
* **Statevector amplitude & probability readouts**
* **Action history log**
* **Level challenge description**



### 🧪 **Measurement & Fidelity Checking**

* Simulate measurements using Qiskit Aer (200 shots)
* Verify fidelity against the target state for each challenge
* Automatically normalize statevectors



## 🖥️ **Screenshots**

![View of home page when app is just opened](/screenshots/home.png?raw=true "Home")
![View of an entangled qubit](/screenshots/ent.png?raw=true "Ent")



## 🧱 **Project Structure**

```
main_final_final_final_glow.py
README.md
```



## 🔧 **Requirements**

Install dependencies:

```bash
pip install qiskit qiskit-aer matplotlib numpy
```

Tkinter is included by default on most systems, but on Linux you may need:

```bash
sudo apt install python3-tk
```



## ▶️ **How to Run**

```bash
python main_final_final_final_glow.py
```

The game window will open with all controls ready to use.



## 🛠️ **Technologies Used**

* **Python 3**
* **Tkinter** (GUI)
* **Matplotlib** (3D visualization)
* **Qiskit + AerSimulator** (quantum circuit simulation)
* **NumPy** (math operations)



## 📚 **Educational Value**

This project is great for learning:

* Fundamentals of multi-qubit states
* Bloch sphere interpretation
* Entanglement and mixed states
* How gates affect statevectors
* How fidelities measure similarity between states
* Hands-on quantum circuit construction



## 🤝 Contributing

Feel free to submit pull requests or open issues if you'd like to add features such as:

* More levels
* Mixed-state challenges
* Custom circuit editor
* Quantum gate tutorials
* Saving/loading circuits



