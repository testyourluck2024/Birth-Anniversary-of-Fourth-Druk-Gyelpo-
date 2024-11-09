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
    </style>
</head>
<body>

    <div class="container">
        <h1>Thank You for Participating!</h1>
        <div class="message-box">
            <p>Your Lucky Draw ticket number has been selected: <strong id="ticketNumberDisplay">[Ticket Number]</strong></p>
            <p>Let’s see the results on November 11, 2024! Results will be announced here on this website.</p>
        </div>

        <div class="results-time">
            <p>Lucky Draw Results will be announced at 5:00 PM on November 11, 2024.</p>
        </div>
    </div>

    <script>
        // Display the ticket number from URL query (for demonstration)
        const params = new URLSearchParams(window.location.search);
        const ticketNumber = params.get('ticketNumber');
        document.getElementById('ticketNumberDisplay').textContent = ticketNumber || '[Ticket Number]';
    </script>

</body>
</html>
