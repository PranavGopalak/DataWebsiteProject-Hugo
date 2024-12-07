---
title: "Random Quote"
draft: false
---

# Motivational Quote

<div id="quote-container">
  <p id="quote">Loading quote...</p>
  <p id="author"></p>
  <button onclick="generateQuote()">New Quote</button>
</div>

<script>
  const quotes = [
    { text: "The best way to predict the future is to invent it.", author: "Alan Kay" },
    { text: "Life is 10% what happens to us and 90% how we react to it.", author: "Charles R. Swindoll" },
    { text: "The only way to do great work is to love what you do.", author: "Steve Jobs" },
  ];

  function generateQuote() {
    const randomIndex = Math.floor(Math.random() * quotes.length);
    const quote = quotes[randomIndex];
    document.getElementById('quote').innerText = `"${quote.text}"`;
    document.getElementById('author').innerText = `— ${quote.author}`;
  }

  window.onload = generateQuote;
</script>
