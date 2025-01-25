# Bitcoin-Dollar-BTCD

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple Website</title>
    <style>
        /* Basic styling */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
        }

        header {
            background-color: #333;
            color: white;
            padding: 20px;
            text-align: center;
        }

        nav {
            background-color: #444;
            overflow: hidden;
            text-align: center;
        }

        nav a {
            display: inline-block;
            color: white;
            text-decoration: none;
            padding: 14px 20px;
        }

        nav a:hover {
            background-color: #575757;
        }

        section {
            padding: 50px;
            display: none;
            text-align: center;
        }

        section.active {
            display: block;
        }

        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }

        /* Responsive design */
        @media (max-width: 600px) {
            nav a {
                display: block;
                text-align: center;
            }
        }
    </style>
</head>
<body>

    <header>
        <h1>My Website</h1>
    </header>

    <nav>
        <a href="javascript:void(0)" onclick="showSection('home')">Home</a>
        <a href="javascript:void(0)" onclick="showSection('about')">About</a>
        <a href="javascript:void(0)" onclick="showSection('media')">Media</a>
        <a href="javascript:void(0)" onclick="showSection('creator')">Creator</a>
    </nav>

    <section id="home" class="active">
        <h2>Welcome to Home</h2>
        <p>This is the home section of the website.</p>
    </section>

    <section id="about">
        <h2>About Us</h2>
        <p>Learn more about our mission and values.</p>
    </section>

    <section id="media">
        <h2>Our Media</h2>
        <p>Explore our media content and galleries.</p>
    </section>

    <section id="creator">
        <h2>Meet the Creator</h2>
        <p>Get to know the person behind this project.</p>
    </section>

    <footer>
        &copy; 2025 My Website. All Rights Reserved.
    </footer>

    <script>
        function showSection(sectionId) {
            var sections = document.querySelectorAll('section');
            sections.forEach(function(section) {
                section.classList.remove('active');
            });
            document.getElementById(sectionId).classList.add('active');
        }
    </script>

</body>
</html>
