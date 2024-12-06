---
title: "Calculator"
---

# Simple Calculator

<!-- Add your calculator HTML and JS here -->

<div id="calculator">
  <input type="number" id="num1" placeholder="Number 1">
  <input type="number" id="num2" placeholder="Number 2">
  <button onclick="addNumbers()">Add</button>
  <p>Result: <span id="result"></span></p>
</div>

<script>
  function addNumbers() {
    const num1 = parseFloat(document.getElementById('num1').value);
    const num2 = parseFloat(document.getElementById('num2').value);
    const sum = num1 + num2;
    document.getElementById('result').innerText = sum;
  }
</script>