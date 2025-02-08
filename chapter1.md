# Neuron and Logic Gates

A **Neuron** leads to the **Neurode** and then the **MCP Neuron**, which can be used to design logic gates like **AND** and **OR** using a formula with appropriate threshold values.

## Activation Function

The formula for the activation function is:

\[
f(y) =
\begin{cases} 
0, & Z < \theta \\
1, & Z \geq \theta
\end{cases}
\]

where:
- \( x_1, x_2 \) are inputs  
- \( Z \) is the summation of inputs  
- \( \theta \) is the threshold  

## Examples:

1. **AND Gate:**  
   - Inputs: \( x_1, x_2 \in \{0,1\} \)  
   - For **θ = 2**, the condition is satisfied, meaning the output is `1` only when both inputs are `1`.

2. **OR Gate:**  
   - Inputs: \( x_1, x_2 \in \{0,1\} \)  
   - For **θ = 1**, the condition is satisfied, meaning the output is `1` when at least one input is `1`.

---

# Frank Rosenblatt's Perceptron

The **perceptron** starts with its **weights** (\( w_1 \) and \( w_2 \)) and **bias** set to zero, representing a line in the **xy** plane. It tries to find a **separating line** that classifies points correctly.

### Learning Process:
- At first, it **makes mistakes**, sometimes classifying circles correctly but not triangles, or vice versa.
- These **incorrect attempts** are shown as **dashed lines**.
- The perceptron **learns from mistakes**, adjusting its weights and bias with each pass through the data.

### Final Classification:
- Eventually, it finds the **best separating line** (shown as a **solid black line**) that correctly divides the two groups.
- The **weights** determine the **slope** of the line.
- The **bias** controls how far the line is from the origin.

---

# Perceptron and Its Evolution

## 1. Perceptron and its Limitations
- Once the perceptron learns the relationship between a person's body weight and height and whether they are obese (`y = +1`) or not (`y = -1`), it can predict new data points.
- However, the perceptron might still make mistakes. Why?
    - **Hint**: Look at the graph — how many different lines can separate the circles from the triangles?
    - Multiple lines might separate the two classes, but the perceptron learns only one possible solution.
    - If the data is not linearly separable, the perceptron cannot find a perfect boundary.
    - **Limitation**: The perceptron works well only when a clear **linear boundary** exists between the two categories.

---

## 2. Perceptron with Multiple Inputs
- A perceptron becomes more complex as the number of inputs increases.
    - With inputs like `x₁`, `x₂`, `x₃`, `x₄`, each adds its own axis.
    - **For 3 inputs** (`x₁`, `x₂`, `x₃`), the data becomes 3D, and a **2D plane** is needed to separate the points.
    - **For 4 or more inputs**, you need a **hyperplane** to separate the data.
    - A **hyperplane** is a generalization of a line or plane in higher dimensions, but it's difficult to visualize beyond 3D.
    - **Key Point**: In higher dimensions, the perceptron requires a hyperplane to separate the data, which is harder to visualize in 3D.

---

## 3. The Mark I Perceptron (1958)
- In 1958, Rosenblatt created the **Mark I Perceptron**, which used multiple perceptron units.
    - It could process an image of **20x20 pixels** (400 total pixels).
    - The Mark I took a long list of input values (`x₁`, `x₂`, ..., `x₄₀₀`) and used a network of artificial neurons with both fixed and learnable weights.
    - The output signal helped identify patterns in the image.
    - It could **learn to recognize letters** encoded in the 400 pixels.
    - Once the Mark I learned, it stored knowledge in the **weights** of its connections.
    - The **Mark I** showcased the potential of neural networks in pattern recognition, sparking significant excitement.

---

## 4. The Limitations of the Perceptron in Reasoning
- The perceptron learns correlations between input values (`x₁`, `x₂`, ..., `x₄₀₀`) and corresponding outputs (`y`), but it does not "understand" or "reason."
    - For example, it distinguishes letters like “B” and “G” based on patterns but without assigning any true meaning to them.
- **Key Question**: Is identifying patterns the same as thinking or reasoning?
    - The perceptron can recognize patterns but does not engage in deeper reasoning like humans do.
    - This raises the ongoing debate about the limits of **deep neural networks**, which evolved from perceptrons.
    - These networks power technologies like **large language models** and **self-driving cars**, but the journey from perceptrons to these technologies has had setbacks and mistakes.
    - Nonetheless, this path forward remains an exciting and fascinating one.

---

## 5. Mathematical Proof for Linearly Separable Data
- Building the perceptron was a significant accomplishment.
- An even bigger achievement was the **mathematical proof** that a **single layer of perceptrons** can always find a **linearly separating hyperplane** if the data is linearly separable.
    - To understand this proof, we need to explore **vectors** and how they help represent data in machine learning.
    - This is our first step into the **mathematics** behind the methods.


 
