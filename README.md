<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Styled Link Example</title>
    <style>
        /* Styling the link */
        a {
            text-decoration: none; /* Removes the underline */
            color: #3498db; /* Sets the link color */
            font-size: 18px; /* Set the font size */
            font-weight: bold; /* Makes the link text bold */
            transition: color 0.3s ease; /* Smooth transition for color change */
        }

        /* Hover effect */
        a:hover {
            color: #e74c3c; /* Change color on hover */
            text-decoration: underline; /* Adds an underline when hovered */
        }

        /* Active link (when clicked) */
        a:active {
            color: #2c3e50; /* Change color when the link is active */
        }

        /* Visited link */
        a:visited {
            color: #8e44ad; /* Change color for visited links */
        }
    </style>
</head>
<body>

    <a href="https://www.example.com" target="_blank">Visit Example Website</a>

</body>
</html>
