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

 
