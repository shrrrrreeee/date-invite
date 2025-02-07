# date-invite
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Will You Go on a Date with Me?</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin-top: 50px;
        }
        h1 {
            font-size: 28px;
        }
        .buttons {
            margin-top: 20px;
        }
        button {
            font-size: 18px;
            padding: 10px 20px;
            margin: 10px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <h1>Will you go on a date with me?</h1>
    <div class="buttons">
        <button onclick="yesClick()">Yes</button>
        <button id="noButton" onclick="noClick()">No</button>
    </div>

    <script>
        let noClickCount = 0;
        function yesClick() {
            alert("Yay! Can't wait for our date! ❤️");
        }
        function noClick() {
            noClickCount++;
            if (noClickCount < 3) {
                alert("Try again! Are you sure?");
            } else {
                alert("No isn't an option anymore 😆");
                document.getElementById("noButton").style.display = "none";
            }
        }
    </script>
</body>
</html>
