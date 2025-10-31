# Quickassist<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Simple Calculator</title>
  <style>
    body {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      background: #f0f4f8;
      font-family: Arial, sans-serif;
    }
    .calculator {
      background: #fff;
      padding: 2rem;
      border-radius: 12px;
      box-shadow: 0 8px 20px rgba(0,0,0,0.1);
      text-align: center;
      width: 300px;
    }
    input {
      width: 100%;
      padding: 0.8rem;
      margin-bottom: 1rem;
      font-size: 1.2rem;
      text-align: right;
      border-radius: 8px;
      border: 1px solid #ccc;
      outline: none;
    }
    button {
      width: 22%;
      padding: 1rem;
      margin: 0.5%;
      font-size: 1.2rem;
      border-radius: 8px;
      border: none;
      cursor: pointer;
      transition: 0.3s;
    }
    button.operator {
      background: #4caf50;
      color: white;
    }
    button.number {
      background: #e0e0e0;
    }
    button:hover {
      opacity: 0.9;
    }
    button.equal {
      background: #2196f3;
      color: white;
    }
  </style>
</head>
<body>
  <div class="calculator">
    <input type="text" id="display" readonly placeholder="0" />
    <div>
      <button class="number" onclick="appendNumber('7')">7</button>
      <button class="number" onclick="appendNumber('8')">8</button>
      <button class="number" onclick="appendNumber('9')">9</button>
      <button class="operator" onclick="appendOperator('/')">/</button>
