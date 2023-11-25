<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
    <div class="container">

        <h1>Password Generator</h1>

        <div class="display-container">

            <input readonly placeholder="Password" class="display" data-passwordDisplay>

            <button data-copy>
                <span data-copyMsg></span>
                <img src="./assets/copy.svg" alt="copy" width="23" height="23">
            </button>

        </div>


        <div class="input-container">

            <!--password length section-->
            <div class="length-container">
                <p>Password Length</p>
                <p data-lengthNumber>0</p>
            </div>
            
            <!--slider-->
            <input type="range" min="1" max="20" class="slider" step="1" data-lengthSlider>

            <!-- checkboxes-->
            <div>
                <input type="checkbox" id="uppercase">
                <label for="uppercase">Includes Uppercase letters</label>
            </div>

            <div>
                <input type="checkbox" id="lowercase">
                <label for="lowercase">Includes Lowercase letters</label>
            </div>

            <div>
                <input type="checkbox" id="numbers">
                <label for="numbers">Includes Numbers </label>
            </div>

            <div>
                <input type="checkbox" id="symbols">
                <label for="symbols">Includes Symbols </label>
            </div>

            <!-- strength section-->
            <div class="strength-container">
                <p>Strength</p>
                <div data-indicator></div>
            </div>

            <!-- generate password-->
            <button class="generateButton">Generate Password</button>

        </div>

    </div>
    <script src="script.js"></script>
</body>
</html>
