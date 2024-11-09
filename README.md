<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lucky Draw Confirmation</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f7f7f7;
            color: #333;
            text-align: center;
        }
        .container {
            max-width: 800px;
            margin: auto;
            padding: 20px;
        }
        h1 {
            color: #4CAF50;
        }
        .message-box {
            background-color: #e9f7ff;
            border: 1px solid #4CAF50;
            padding: 20px;
            margin: 20px 0;
            border-radius: 8px;
            font-size: 18px;
            font-weight: bold;
            color: #333;
        }
        .results-time {
            font-size: 18px;
            font-weight: bold;
            color: #333;
            margin-top: 20px;
        }
        .form-box {
            margin: 20px 0;
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>Lucky Draw Participation</h1>

        <!-- Ticket Selection Form -->
        <div class="form-box" id="formBox">
            <form onsubmit="submitTicketNumber(event)">
                <label for="ticketNumber">Select Your Ticket Number:</label>
                <input type="text" id="ticketNumber" name="ticketNumber" required>
                <button type="submit">Submit</button>
            </form>
        </div>

        <!-- Confirmation Message (Initially Hidden) -->
        <div class="message-box" id="confirmationBox" style="display: none;">
            <p>Your Lucky Draw ticket number has been selected: <strong id="ticketNumberDisplay">[Ticket Number]</strong></p>
            <p>Let’s see the results on November 11, 2024! Results will be announced here on this website.</p>
        </div>

        <div class="results-time">
            <p>Lucky Draw Results will be announced at 5:00 PM on November 11, 2024.</p>
        </div>
    </div>

    <script>
        function submitTicketNumber(event) {
            event.preventDefault();
            const ticketNumber = document.getElementById("ticketNumber").value;

            // Display the confirmation message with the ticket number
            document.getElementById("ticketNumberDisplay").textContent = ticketNumber;
            document.getElementById("formBox").style.display = "none";  // Hide the form
            document.getElementById("confirmationBox").style.display = "block";  // Show confirmation box
        }
    </script>

</body>
</html>
