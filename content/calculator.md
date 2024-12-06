---
title: "Calculator"
date: 2024-12-01T12:00:00Z
draft: false
---

## Simple Calculator

<form id="calculator-form">
  <input type="number" id="num1" placeholder="First Number" required>
  <input type="number" id="num2" placeholder="Second Number" required>
  <button type="submit">Calculate</button>
</form>

<h3 id="result"></h3>

<script>
  document.getElementById('calculator-form').addEventListener('submit', function(e) {
    e.preventDefault();
    const num1 = parseFloat(document.getElementById('num1').value);
    const num2 = parseFloat(document.getElementById('num2').value);
    if (!isNaN(num1) && !isNaN(num2)) {
      const sum = num1 + num2;
      document.getElementById('result').innerText = `Result: ${sum}`;
    } else {
      document.getElementById('result').innerText = "Please enter valid numbers.";
    }
  });
</script>