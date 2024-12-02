---
title: Calculator
parent: Plugins
nav_order: 7
---

# Calculator Plugin Documentation

The Calculator is a powerful tool built on [Math.js](https://mathjs.org/), offering quick and advanced mathematical computations. It supports a wide range of features, from simple arithmetic to unit conversions and variable handling.

## **Features**

### **1. Perform Advanced Calculations**
Use the calculator to handle:
- Basic arithmetic: `5 + 3`, `12 / 4`
- Trigonometry: `sin(30°)`, `cos(pi/3)`
- Statistics: `mean(5, 10, 15)`, `std(4, 7, 9)`
- Complex numbers: `2 + 3i`, `abs(3 + 4i)`
- And more advanced mathematical functions provided by Math.js.

### **2. Work with Variables**
- Assign variables within calculations, e.g., `x = 5`, `y = x * 2`.
- Refer to the **last result** using `ans`. For example:
  ``` 
  5 * 2  
  ans + 3  
  ```  
- Access specific results using `$<number>` notation, where `<number>` corresponds to the calculation's position in the history. For example:
  ```
  $3 * 2  
  ```  
  (Fetches the result from the third calculation.)

### **3. Modify Previous Calculations**
Easily revisit and adjust past calculations by clicking on them in the history. This allows you to refine inputs and recalculate effortlessly.

### **4. Convert Between Units**
Seamlessly convert between various units of measurement. Examples include:
- Length: `5 cm to inches`
- Weight: `10 kg to pounds`
- Time: `2 hours to minutes`
- Temperature: `100 °C to °F`
- Volume: `1 liter to gallons`

### **5. Interactive Interface**
- Calculation history is preserved, making it easy to track and reuse results.
- The plugin highlights errors and offers suggestions for corrections.