### Flask Application Design for Calculating Machine Efficiency

### HTML Files

1. **index.html**:
   - This file serves as the homepage of the application.
   - It contains an HTML form with fields for the following inputs:
     - Object Weight (in newtons)
     - Effort Applied (in newtons)
     - Machine Efficiency (in percentage)
   - It also includes a button labeled "Calculate" that triggers the calculation process.

2. **results.html**:
   - This file displays the calculated results.
   - It contains HTML elements to display the following:
     - Mechanical Advantage of the Machine
     - Work Done by the Machine (in joules)
     - Work Lost Due to Friction (in joules)

### Routes

1. **route for the homepage**:
   - This route is responsible for handling requests to the homepage (index.html).
   - It renders the index.html file.

2. **route for calculating and displaying results**:
   - This route is triggered when the "Calculate" button is clicked on the homepage.
   - It extracts the input values from the request object.
   - It calculates the mechanical advantage, work done by the machine, and work lost due to friction using appropriate formulas.
   - It renders the results.html file, passing the calculated values as arguments.

### Formulae to Calculate Mechanical Advantage and Work

- Mechanical Advantage = (Object Weight) / (Effort Applied)
- Work Done by Machine = (Mechanical Advantage) * (Effort Applied)
- Work Lost Due to Friction = (Input Work) - (Work Done by Machine)

### Outline of the Flask Application Design

1. Create a Flask app instance.
2. Define the routes for the homepage and results page.
3. In the homepage route, render the index.html file.
4. In the results route:
   - Extract input values from the request object.
   - Calculate the mechanical advantage, work done by the machine, and work lost due to friction using the provided formulae.
   - Render the results.html file, passing the calculated values as arguments.
5. Run the Flask application.

This design provides a structured approach to solving the problem using Python Flask. The user inputs values via the HTML form, and the Flask application calculates and displays the results on the results page.