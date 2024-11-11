
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lucky Draw Announcement</title>
    <style>
        /* Container with background image */
        .container {
            background-image: url('path-to-your-uploaded-image.jpg'); /* Replace with your image URL */
            background-size: cover;
            background-position: center;
            position: relative;
            padding: 20px;
            color: black; /* Default color for text */
        }
        
        /* Light overlay for readability */
        .container::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background-color: rgba(255, 255, 255, 0.5); /* Light overlay */
            z-index: 1;
        }
        
        /* Ensuring content is above the background */
        .container > * {
            position: relative;
            z-index: 2;
        }

        /* Style for announcement section */
        .announcement {
            font-weight: bold;
            font-size: 1.2em;
            text-align: center;
            margin-bottom: 20px;
            color: red; /* Set entire announcement text to red */
        }

        /* Style for the main topic */
        h1, h2 {
            color: green; /* Topic in green */
        }

        /* Subsection heading */
        h3 {
            color: blue; /* Subsection color */
        }

        /* Paragraph text */
        p {
            color: darkblue; /* Paragraph text color */
        }

        /* Make sure to highlight all announcement sentences in red */
        .announcement p {
            color: red; /* Announcement text in red */
        }

        /* Payment Note Box */
        .payment-note {
            background-color: lightyellow;
            padding: 10px;
            border: 1px solid orange;
            color: darkred;
            font-weight: bold;
            text-align: center;
        }

        /* TRC20 Address Box with Copy Button */
        .trc20-address p {
            color: darkblue;
            font-weight: bold;
            text-align: center;
        }
        .trc20-address textarea {
            font-size: 16px;
            text-align: center;
            color: black;
            width: 100%;
        }
        .copy-button {
            background-color: orange;
            color: white;
            border: none;
            padding: 8px 12px;
            font-weight: bold;
            cursor: pointer;
            margin-top: 10px;
            display: block;
            width: 100%;
        }

        /* Telegram button */
        .telegram-button {
            display: block;
            background-color: #0088cc;
            color: white;
            text-align: center;
            padding: 10px 20px;
            border-radius: 8px;
            font-size: 16px;
            font-weight: bold;
            text-decoration: none;
            margin: 20px auto;
            width: 200px;
            cursor: pointer;
        }
        .telegram-button:hover {
            background-color: #0077b3;
        }

        /* Important note */
        .strict-note {
            font-weight: bold;
            color: darkred;
            text-align: center;
            background-color: lightcoral;
            padding: 10px;
            margin-top: 20px;
        }

        /* Results Time */
        .results-time {
            color: darkgreen;
            text-align: center;
            margin-top: 20px;
            font-weight: bold;
        }

    </style>
</head>
<body>

<div class="container">
    <!-- Announcement Banner -->
    <div class="announcement">
        <p>Announcement: The lucky draw results will be announced on the website on November 11, 2024, at 5:00 PM.</p>
    </div>

    <!-- Main Content -->
    <h1>མི་དབང་མཆོག་གི་ སྐུའི་འཁྲུངས་སྐར་ལུ་བཀྲ་ཤིས་བདེ་ལེགས།</h1>
    <h2>NOVEMBER 11, 2024 HAPPY BIRTHDAY YOUR MAJESTY</h2>
    <h3>LUCKY DRAW CONDUCTED BY "Bhutan Crypto Currency Intelligence Agencies (BCCIA)"</h3>
    <p>Enter your details for a chance to win $1000 on the Birth Anniversary of the Fourth Druk Gyelpo! The Lucky Draw will be open from November 8, 2024 to November 11, 2024, so make sure to participate before it's too late!</p>

    <!-- Payment Note Box -->
    <div class="payment-note">
        <p><strong>Payment: $5</strong> to win $1000! Don't miss your chance. Deadline: November 11, 2024.</p>
    </div>

    <!-- TRC20 Address Box with Copy Button -->
    <div class="trc20-address">
        <p>Send payment to the following TRC20 address:</p>
        <textarea id="trc20Address" readonly rows="3">TMuWGYnqYxGSXgD9sfe3m1aUfNk2JW8Aci</textarea>
        <button class="copy-button" onclick="copyToClipboard()">Copy Address</button>
    </div>

    <!-- Form Container -->
    <div class="form-container">
        <form action="#" method="post">
            <label for="ticketNumber">Enter Ticket Number (A1 to A5000000):</label>
            <input type="text" id="ticketNumber" name="ticketNumber" required>

            <label for="dzongkhag">Select Dzongkhag:</label>
            <select id="dzongkhag" name="dzongkhag" required>
                <option value="Paro">Paro</option>
                <option value="Thimphu">Thimphu</option>
                <option value="Haa">Haa</option>
                <option value="Gasa">Gasa</option>
                <option value="Chukha">Chukha</option>
                <option value="Mongar">Mongar</option>
                <option value="Lhuntse">Lhuntse</option>
                <option value="Samtse">Samtse</option>
                <option value="Dagana">Dagana</option>
                <option value="Zhemgang">Zhemgang</option>
                <option value="Sarpang">Sarpang</option>
                <option value="Trongsa">Trongsa</option>
                <option value="Samdrupjongkhar">Samdrupjongkhar</option>
                <option value="Trashigang">Trashigang</option>
                <option value="Trashiyangtse">Trashiyangtse</option>
                <option value="Tsirang">Tsirang</option>
                <option value="Punakha">Punakha</option>
                <option value="Wangduephodrang">Wangduephodrang</option>
            </select>

            <label for="fullName">Your Full Name:</label>
            <input type="text" id="fullName" name="fullName" required>

            <label for="contactNumber">Your Contact Number:</label>
            <input type="text" id="contactNumber" name="contactNumber" required>

            <label for="paymentScreenshot">Upload Payment Screenshot:</label>
            <input type="file" id="paymentScreenshot" name="paymentScreenshot" required>

            <button type="submit">Submit</button>
        </form>
    </div>

    <!-- Telegram Contact Button -->
    <a href="https://t.me/bcciateam" target="_blank" class="telegram-button">
        Contact Support on Telegram
    </a>

    <!-- Strict Note -->
    <div class="strict-note">
        <p><strong>Important:</strong> Fake transactions or screenshots will be strictly prohibited by the system. TASHIDELAK TO EVERYONE!</p>
    </div>

    <!-- Results Time -->
    <div class="results-time">
    </div>
</div>

<script>
    function copyToClipboard() {
        var copyText = document.getElementById("trc20Address");
        copyText.select();
        copyText.setSelectionRange(0, 99999); /* For mobile devices */
        document.execCommand("copy");
        alert("Address copied to clipboard!");
    }
    
    <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Access Lucky Draw Page</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 20px;
        }
        .qr-code {
            margin: 20px 0;
        }
        .link-button, .qr-code img {
            border-radius: 8px;
            padding: 10px 20px;
            color: white;
            text-decoration: none;
            font-size: 16px;
            font-weight: bold;
            cursor: pointer;
            margin-top: 10px;
        }
        .link-button {
            background-color: #0088cc;
        }
    </style>
</head>
<body>

    <h1>Access the Lucky Draw Page</h1>
    <p>You have multiple ways to visit the page:</p>

    <!-- Shortened Link -->
    <p>
        <a href="https://bit.ly/your-shortened-link" target="_blank" class="link-button">
            Visit Lucky Draw Page (Shortened Link)
        </a>
    </p>

    <!-- Landing Page Redirect Link -->
    <p>If the above link doesn't work, you can try this one:</p>
    <a href="https://your-landing-page.com" target="_blank" class="link-button">
        Alternative Link
    </a>

    <!-- QR Code -->
    <div class="qr-code">
        <h2>Scan the QR Code</h2>
        <p>Alternatively, scan this QR code to access the page directly:</p>
        <img id="qrCode" src="" alt="QR Code">
    </div>

    <!-- QR Code Generator Script -->
    <script>
        const link = "https://your-main-link.com";
        const qrCodeImg = document.getElementById("qrCode");
        qrCodeImg.src = `https://chart.googleapis.com/chart?chs=150x150&cht=qr&chl=${encodeURIComponent(link)}`;
    </script>

</body>
</html>
