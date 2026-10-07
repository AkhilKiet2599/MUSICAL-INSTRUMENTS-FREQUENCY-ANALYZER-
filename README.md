🎵 Musical Instrument Frequency Analyzer

📌 Overview

The Musical Instrument Frequency Analyzer is a B.Tech Mathematics mini project that demonstrates how eigenvalues and eigenvectors can be used to analyze vibrations.

The project models a small two-mass spring/string system, calculates its natural frequencies, and visualizes its first vibration modes.

The project is designed to be simple, interactive, beginner-friendly, and completely free to run in Google Colab.

---

🎯 Problem Statement

«Model a small spring-mass/string system and visualize its first modes.»

The user enters simple physical parameters such as mass and spring stiffness.

The program then:

1. Constructs the mathematical matrices.
2. Calculates eigenvalues and eigenvectors.
3. Finds natural frequencies.
4. Displays the mathematical calculations.
5. Visualizes the vibration modes.
6. Validates the result using a known test case.

---

🧮 Mathematical Topic

Eigenvalues & Vibration Modes

The system is represented by:

[
M\ddot{x}+Kx=0
]

where:

- (M) = Mass matrix
- (K) = Stiffness matrix
- (x) = Displacement vector

For a two-mass system:

[
M=
\begin{bmatrix}
m_1&0\
0&m_2
\end{bmatrix}
]

and

[
K=
\begin{bmatrix}
k_1+k_2&-k_2\
-k_2&k_2
\end{bmatrix}
]

The vibration problem becomes:

[
K\phi=\lambda M\phi
]

where:

- (\lambda) = Eigenvalue
- (\phi) = Eigenvector

The eigenvalue is related to angular frequency by:

[
\lambda=\omega^2
]

Therefore:

[
\omega=\sqrt{\lambda}
]

and the natural frequency is:

[
\boxed{f=\frac{\sqrt{\lambda}}{2\pi}}
]

Key idea

[
\boxed{\text{Eigenvalues} \rightarrow \text{Natural Frequencies}}
]

[
\boxed{\text{Eigenvectors} \rightarrow \text{Vibration Modes}}
]

---

🔄 Project Workflow

Simple Inputs
     ↓
Mass & Stiffness Matrices
     ↓
Eigenvalue Problem
     ↓
Eigenvalues + Eigenvectors
     ↓
Natural Frequencies
     ↓
Vibration Modes
     ↓
Graphs & Visualization
     ↓
Validation

---

🛠️ Technologies Used

- Python
- Google Colab / Jupyter Notebook
- NumPy
- Matplotlib

Cost

Free

APIs

Not required

Secret Keys

Not required

Paid Software

Not required

---

🚀 How to Run

1. Open Google Colab

Visit:

https://colab.research.google.com/

2. Upload the notebook

Upload:

Musical_Instrument_Frequency_Analyzer.ipynb

3. Run the cells

Run the notebook from top to bottom.

The notebook is organized into small sections so beginners can understand each step.

4. Enter values

Change the mass and stiffness values when prompted.

5. View the results

The notebook will display:

- Mass matrix
- Stiffness matrix
- Eigenvalues
- Eigenvectors
- Natural frequencies
- Vibration-mode graphs
- Validation results

---

🎛️ Inputs

The project uses four basic parameters.

Parameter| Meaning| Example
"m1"| Mass 1| 1 kg
"m2"| Mass 2| 1 kg
"k1"| Spring stiffness 1| 100 N/m
"k2"| Spring stiffness 2| 100 N/m

Example:

m1 = 1.0
m2 = 1.0
k1 = 100.0
k2 = 100.0

Changing these values changes the calculated frequencies and vibration modes.

---

📊 Main Outputs

1. Mass Matrix

[
M=
\begin{bmatrix}
m_1&0\
0&m_2
\end{bmatrix}
]

2. Stiffness Matrix

[
K=
\begin{bmatrix}
k_1+k_2&-k_2\
-k_2&k_2
\end{bmatrix}
]

3. Eigenvalues

The program calculates:

[
\lambda_1,\lambda_2
]

These determine the natural frequencies.

4. Eigenvectors

The eigenvectors describe the corresponding vibration modes.

5. Natural Frequencies

The program calculates:

[
f=\frac{\sqrt{\lambda}}{2\pi}
]

and displays the frequency in Hz.

6. Visualization

The program plots the vibration modes and natural frequencies.

---

🧪 Known Test Case

For validation, use:

m1 = 1 kg
m2 = 1 kg
k1 = 100 N/m
k2 = 100 N/m

The matrices are:

[
M=
\begin{bmatrix}
1&0\
0&1
\end{bmatrix}
]

[
K=
\begin{bmatrix}
200&-100\
-100&100
\end{bmatrix}
]

Expected eigenvalues:

[
\lambda_1\approx38.1966
]

[
\lambda_2\approx261.8034
]

Expected natural frequencies:

[
\boxed{f_1\approx0.9836\text{ Hz}}
]

[
\boxed{f_2\approx2.5751\text{ Hz}}
]

Therefore, the expected output is approximately:

Mode 1: 0.9836 Hz
Mode 2: 2.5751 Hz

Small differences in the final decimal places are normal due to numerical calculations.

---

✅ Automatic Validation

The notebook contains a validation section that compares the calculated results with the known test case.

The implementation is considered correct when the calculated frequencies are approximately:

0.9836 Hz
2.5751 Hz

---

📈 Visualization

The project visualizes the first two vibration modes.

Mode 1

The masses generally move together in the same direction.

Mode 2

The masses generally move in opposite directions.

The graphs change when the input parameters are changed.

This makes the relationship between physical parameters → eigenvalues → vibration modes easy to understand.

---

🎵 Connection to Musical Instruments

Musical instruments produce sound through vibration.

Examples include:

- 🎸 Guitar
- 🎻 Violin
- 🎹 Piano
- 🥁 Drums

Each vibrating system has characteristic natural frequencies and vibration modes.

Our spring-mass model is a simplified mathematical representation that helps demonstrate these concepts.

---

🌍 Real-World Applications

The same mathematical principles are used in:

- Musical instrument design
- Acoustics
- Mechanical engineering
- Structural vibration analysis
- Automotive engineering
- Aerospace engineering
- Robotics
- Machine design

---

🧠 Learning Outcomes

After completing this project, students can understand:

- Matrix representation of physical systems
- Eigenvalues
- Eigenvectors
- Natural frequency
- Vibration modes
- Numerical computation using Python
- Data visualization
- Applications of linear algebra

---

🔧 Project Development Route

Understand
    ↓
AI Vibe Code
    ↓
Validate
    ↓
Customise
    ↓
Document
    ↓
Demo

Understand

Study eigenvalues, eigenvectors and vibration modes.

AI Vibe Code

Create the Python implementation using NumPy and Matplotlib.

Validate

Test the program using the known mathematical example.

Customise

Experiment with different masses and stiffness values.

Document

Record the mathematical model, results and applications.

Demo

Change the input values during the presentation and show how the frequencies and modes change.

---

🎤 Demo Script

«"Our project is the Musical Instrument Frequency Analyzer. It models a small two-mass spring system to study vibration. We construct the mass and stiffness matrices and solve the eigenvalue problem. The eigenvalues determine the natural frequencies, while the eigenvectors represent the vibration modes. By changing the masses or spring stiffness, we can observe how the frequencies and vibration patterns change. This demonstrates a practical application of eigenvalues and eigenvectors in musical acoustics and vibration analysis."»

---

📁 Project Files

Musical-Instrument-Frequency-Analyzer/
│
├── Musical_Instrument_Frequency_Analyzer.ipynb
│
└── README.md

---

🚀 Future Improvements

Possible future versions could include:

- 🎚️ Interactive sliders
- ▶️ Animated vibration modes
- 🎵 Real-time sound generation
- 🎸 Guitar-string simulation
- 🎹 Piano-string simulation
- 📊 Frequency spectrum analysis
- 🔊 Audio input
- 🌐 Interactive browser interface

---

🏁 Conclusion

The Musical Instrument Frequency Analyzer connects mathematical theory with a practical vibration problem.

The project demonstrates:

[
\boxed{\text{Matrices}}
\rightarrow
\boxed{\text{Eigenvalues}}
\rightarrow
\boxed{\text{Natural Frequencies}}
]

and

[
\boxed{\text{Eigenvectors}}
\rightarrow
\boxed{\text{Vibration Modes}}
]

It provides a simple way for beginners to understand how linear algebra can be applied to vibration, engineering, and musical acoustics.

---

📌 Project Summary

Item| Details
Project| Musical Instrument Frequency Analyzer
Problem| Model a small spring-mass/string system and visualize its first modes
Math Topic| Eigenvalues & Vibration Modes
Language| Python
Platform| Google Colab / Jupyter
Libraries| NumPy, Matplotlib
Input| Masses & spring stiffness
Output| Eigenvalues, eigenvectors, frequencies & mode graphs
Validation| Included
APIs| None
Secret Keys| None
Cost| Free
