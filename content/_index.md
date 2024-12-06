---
title: "Home"
date: 2024-12-01T12:00:00Z
draft: false
---

## Welcome to My Website

This website showcases interactive features built with Hugo and JavaScript.

<div id="greeting"></div>

<script>
  const now = new Date();
  const hours = now.getHours();
  let greeting;

  if (hours < 12) {
    greeting = "Good Morning!";
  } else if (hours < 18) {
    greeting = "Good Afternoon!";
  } else {
    greeting = "Good Evening!";
  }

  document.getElementById('greeting').innerText = greeting;
</script>
