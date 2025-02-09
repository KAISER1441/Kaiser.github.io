# Kaiser.github.io
ego slayer club

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ego Slayers - Select Your Team and Position</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #2c3e50;
            color: white;
            text-align: center;
            margin: 0;
            padding: 0;
        }

        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 50px;
        }

        h1 {
            font-size: 3em;
            margin-bottom: 30px;
        }

        select {
            font-size: 1.2em;
            padding: 10px;
            width: 250px;
            margin-top: 20px;
            background-color: #34495e;
            border: none;
            color: white;
        }

        button {
            padding: 15px 25px;
            font-size: 1.2em;
            margin-top: 30px;
            background-color: #e74c3c;
            border: none;
            color: white;
            cursor: pointer;
        }

        button:hover {
            background-color: #c0392b;
        }

        footer {
            margin-top: 50px;
            font-size: 1em;
            color: #bdc3c7;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Ego Slayers</h1>
        <p>Welcome to the Ego Slayers site! Select your club and position below:</p>

        <div>
            <label for="clubSelect">Choose your club:</label>
            <select id="clubSelect">
                <option value="Barcha">Barcha</option>
                <option value="UBERS">UBERS</option>
                <option value="BASTARD MUNCHEN">BASTARD MUNCHEN</option>
                <option value="PXG">PXG</option>
                <option value="MANSHINE">MANSHINE</option>
                <option value="ROYAL MADRID">ROYAL MADRID</option>
            </select>
        </div>

        <div>
            <label for="positionSelect">Choose your position:</label>
            <select id="positionSelect">
                <option value="CF">CF</option>
                <option value="CM">CM</option>
                <option value="WING">WING</option>
                <option value="GK">GK</option>
            </select>
        </div>

        <button onclick="selectTeamAndPosition()">Select Team and Position</button>

        <p id="confirmationMessage" style="display:none; margin-top: 20px;"></p>
    </div>

    <footer>
        <p>&copy; 2025 Ego Slayers. All rights reserved.</p>
    </footer>

    <script>
        function selectTeamAndPosition() {
            const selectedClub = document.getElementById('clubSelect').value;
            const selectedPosition = document.getElementById('positionSelect').value;
            const confirmationMessage = document.getElementById('confirmationMessage');
            
            confirmationMessage.textContent = "You have selected " + selectedClub + " and your position is " + selectedPosition + "!";
            confirmationMessage.style.display = "block";
        }
    </script>
</body>
</html>
