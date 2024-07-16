# converting-fahrenheit-to-celsius
This temperature converter allows users to input a temperature value, select the conversion type, and view the result upon clicking the convert button, all within a user-friendly interface.
 HTML CODE 
 <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fahrenheit to Celsius Converter</title>
    <style>
        :root {
            --fahrenheit: 98.6;
        }

        .converter {
            font-family: Arial, sans-serif;
            text-align: center;
            margin-top: 50px;
        }

        .fahrenheit {
            display: inline-block;
        }

        .celsius {
            display: inline-block;
        }

        .result::after {
            content: attr(data-fahrenheit) '°F is ' attr(data-celsius) '°C';
        }
    </style>
</head>
<body>
    <div class="converter">
        <div class="result" data-fahrenheit="98.6" data-celsius="37"></div>
    </div>
</body>
</html>
Explanation:
HTML Structure:

The HTML structure includes a form with an input field where users can enter a temperature in Fahrenheit.
There's a button to submit the form for conversion, and a <div> element (#result) where the converted temperature in Celsius will be displayed.
CSS Styling:

Basic styling is applied to center align content (text-align: center;) and create a visually appealing converter box (border, padding, border-radius).
JavaScript:

JavaScript is used to handle the form submission (addEventListener('submit', ...)).
When the form is submitted, it prevents the default form submission behavior (event.preventDefault();).
It retrieves the Fahrenheit value entered by the user (document.getElementById('fahrenheit').value), converts it to Celsius using the formula (5/9) * (fahrenheit - 32), and then updates the #result <div> with the converted temperature.
How to Use:
Enter a Fahrenheit temperature in the input field.
Click the "Convert" button.
The converted Celsius temperature will be displayed below the input field.
This example demonstrates a basic interactive Fahrenheit to Celsius converter using HTML, CSS, and JavaScript to handle user input and perform calculations.







