<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Banner Example</title>
    <style>
        body, html {
            margin: 0;
            padding: 0;
            height: 100;
        }

        .banner {
            width: 1200px;
            height: 300px;
            background-image: url('your-image-url.jpg'); /* Replace with your image URL */
            background-size: cover;
            background-position: center;
            text-align: center;
            color: white;
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
        }

        .banner h1 {
            font-size: 36px;
            margin: 0;
        }

        .banner p {
            font-size: 18px;
            margin-top: 10px;
        }
    </style>
</head>
<body>

    <div class="banner">
        <h1>Welcome to Our Website!</h1>
        <p>We provide amazing services just for you.</p>
    </div>

</body>
</html>
