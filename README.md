<!DOCTYPE html>
<html lang="en">
<head>
    <style>
        /* Reset default margin and padding */
        body, html {
            margin: 0;
            padding: 0;
            font-family: Arial, sans-serif;
        }

        /* Styling the navigation bar */
        .navbar {
            background-color: #0e194d; /* Dark background color */
            overflow: hidden; /* Ensures the content is contained within the navbar */
            text-align: center; /* Centers the links */
        }

        /* Styling each link inside the navbar */
        .navbar a {
            display: inline-block; /* Display links horizontally */
            padding: 14px 20px; /* Padding inside each link */
            text-decoration: none; /* Removes underline from links */
            color: white; /* White text color */
            font-size: 16px; /* Font size for the links */
            transition: background-color 0.3s ease; /* Smooth transition for background color change */
        }

        /* Hover effect for the links */
        .navbar a:hover {
            background-color: #ddd; /* Light background when hovered */
            color: black; /* Change text color when hovered */
        }

        /* Active link styling (when a link is clicked or active) */
        .navbar a.active {
            background-color: #004AAD; /* Blue background for active link */
            color: white; /* Keep text white for active link */
        }

        /* Hamburger menu icon styling */
        .navbar .icon {
            z-index: 2;
            display: none;
            font-size: 30px;
            color: white;
            padding: 14px 20px;
            background-color: #333;
            cursor: pointer;
        }

        /* For small screens (mobile devices) */
        @media screen and (max-width: 768px) {
            .navbar a {
                display: none; /* Hide the links by default */
                width: 100%; /* Make the links take full width */
                text-align: left; /* Align links to the left */
                padding: 14px; /* Adjust padding for the links */
            }

            .navbar a.active {
                background-color: #4CAF50;
                color: white;
            }

            /* Display the hamburger icon */
            .navbar .icon {
                display: block;
            }

            /* When the hamburger icon is clicked, show the links */
            .navbar.responsive a {
                display: block;
            }

            .navbar.responsive .icon {
                position: absolute;
                right: 0;
                top: 0;
            }
        }

        /* Styling for the header with sparkle effect */
        .header {
            background-color: #0e194d;
            color: white;
            padding: 20px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        /* Sparkle Effect */
        .header::before, .header::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url('https://media.giphy.com/media/1g0mXL8l7hOQk9Znyh/giphy.gif') repeat;
            opacity: 0.1;
            animation: sparkle 1s linear infinite;
            z-index: 1;
        }

        /* Keyframes for sparkle animation */
        @keyframes sparkle {
            0% {
                transform: scale(1);
                opacity: 0.1;
            }
            50% {
                transform: scale(1.1);
                opacity: 0.4;
            }
            100% {
                transform: scale(1);
                opacity: 0.1;
            }
        }

        /* Header Text */
        .header h1 {
            position: relative;
            z-index: 2;
        }
    </style>
</head>
<body>
    <!-- Header with sparkle effect -->
    <div class="header">
        <h1>Your Sparkling Header</h1>
    </div>

    <!-- Top Navigation Bar -->
    <div class="navbar" id="myNavbar">
        <a href="#home" class="active">Koti</a>
        <a href="#Meista">Meistä</a>
        <a href="#services">Yritys</a>
        <a href="#contact">Palvelut</a>
        <a href="#contact">Koulutus</a>
        <!-- Hamburger Icon -->
        <a href="javascript:void(0);" class="icon" onclick="toggleNavbar()">&#9776;</a>
    </div>

    <script>
        /* Function to toggle the navbar on small screens */
        function toggleNavbar() {
            var navbar = document.getElementById("myNavbar");
            navbar.classList.toggle("responsive");
        }
    </script>
</body>
</html>
