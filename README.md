# Ex.05 Design a Website for Server Side Processing
## Date: 28-04-24
## Name: Shyam R
## Roll.no: 212223040200
## Dept: CSE
## AIM:
To design a website to find surface area of a Right Cylinder in server side.

## FORMULA:
Surface Area = 2Πrh + 2Πr<sup>2</sup>
<br>r --> Radius of Right Cylinder
<br>h --> Height of Right Cylinder

## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Create python programs for views and urls to perform server side processing.

### Step 5:
Create a HTML file to implement form based input and output.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
math.html

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Cylinder Surface Area Calculator</title>
<style>
    body {
        font-family: Arial, sans-serif;
        margin: 0;
        padding: 0;
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
        background-color: black;
    }
    #calculator {
        text-align: center;
        background-color: white;
        padding: 20px;
        border-radius: 10px;
    }
    form {
        margin-bottom: 20px;
    }
    .input-container {
        margin-bottom: 10px;
    }
    label {
        display: block;
        margin-bottom: 5px;
    }
    input[type="number"] {
        width: 100px;
        padding: 8px;
        box-sizing: border-box;
    }
    button {
        background-color: #4CAF50;
        color: white;
        padding: 10px 20px;
        border: none;
        border-radius: 4px;
        cursor: pointer;
    }
    button:hover {
        background-color: #45a049;
    }
    #result {
        font-size: 18px;
        font-weight: bold;
    }
</style>
</head>
<body>

<div id="calculator">
    <h2>Cylinder Surface Area Calculator</h2>
    <h3>Suriya Pravin M(212223230223)</h3>
    <form id="cylinderForm">
        <div class="input-container">
            <label for="radius">Radius:</label>
            <input type="number" id="radius" required>
        </div>
        <div class="input-container">
            <label for="height">Height:</label>
            <input type="number" id="height" required>
        </div>
        <button type="submit">Calculate</button>
    </form>

    <div id="result">Surface Area: <span id="surfaceArea"></span></div>
</div>

<script>
document.getElementById("cylinderForm").addEventListener("submit", function(event) {
    event.preventDefault();
    var radius = parseFloat(document.getElementById("radius").value);
    var height = parseFloat(document.getElementById("height").value);
    var surfaceArea = 2 * Math.PI * radius * (radius + height);
    document.getElementById("surfaceArea").innerText = surfaceArea.toFixed(2);
});
</script>

</body>
</html>

```


## SERVER SIDE PROCESSING:
![alt text](<Screenshot 2024-04-18 120618.png>)

## HOMEPAGE:
![alt text](<Screenshot 2024-05-08 161342.png>)

## RESULT:
The program for performing server side processing is completed successfully.
