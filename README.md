# Tax-Calculator
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Tax-Calculator</title>
        <link rel="stylesheet" href="styles.css">

        <link href="css/styles.css" rel="stylesheet">
        <link rel="preconnect" href="https://fonts.googleapis.com">
        <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
        <link href="https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap" rel="stylesheet">
    </head>
    <body>
        <div class="container">
            <h1>Tax Calculator</h1>
            <div class="Calculator">
                <label for="income">Enter gross annual income</label>
                <input type="number" id="income" placeholder="Enter gross annual income">
            </div>
            <div class="calculator">
                <label for="income">Enter extra income</label>
                <input type="number" id="income" placeholder="Enter extra income">
            </div>
            <div class="calculator">
                <label for="ageGroup">Enter Age group</label>
                <select id="ageGroup">
                    <option value="<40">&lt; 40</option>
                    <option value=">=40<60">&ge; 40 &amp; &lt; 60</option>
                    <option value=">=60">&ge; 60</option>
                </select>
                <span class="error-icon" id="ageError" title="Age Group is mandatory">!</span>

                <button onclick="validateInputs()">Submit</button>
            </div>
        </div>

        <div id="modal" class="modal">
            <div class="modal-content">
                <span class="close" onclick="closeModal()">&times;</span>
                <h2>Your overall income will be</h2>
                <div id="result"></div>
            </div>
        </div>

        <script src="script.js"></script>
    </body>
</html>
