<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Toggle Sections Example</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
        }
        nav {
            background-color: #333;
            padding: 10px;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }
        nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
            font-size: 18px;
            cursor: pointer;
        }
        section {
            display: none;
            padding: 60px 20px;
            margin-top: 50px;
        }
        h2 {
            margin-top: 0;
        }
        .visible {
            display: block;
        }
    </style>
</head>
<body>

    <!-- Navigation Bar with Links -->
    <nav>
        <a onclick="showSection('about')">About</a>
        <a onclick="showSection('experience')">Experience</a>
        <a onclick="showSection('contact')">Contact</a>
    </nav>

    <!-- About Section -->
    <section id="about">
        <h2>About Me</h2>
        <p>
            Welcome to my personal webpage! I'm a passionate professional with expertise in engineering management, product development, and more. My journey in the tech industry has been driven by a love for innovation and a commitment to delivering high-quality solutions.
        </p>
    </section>

    <!-- Experience Section -->
    <section id="experience">
        <h2>Experience</h2>
        <p>
            I have over 10 years of experience in the tech industry, working across various roles and projects. My most recent position was as a Senior Engineering Manager at a leading e-commerce company, where I led a team of engineers to deliver scalable and efficient solutions.
        </p>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <h2>Contact Me</h2>
        <p>
            If you'd like to get in touch, please feel free to reach out via email at vartikashah27@gmail.com or connect with me on LinkedIn. I'm always open to discussing new opportunities, collaborations, or just having a chat about the industry.
        </p>
    </section>

    <!-- JavaScript to Toggle Sections -->
    <script>
        function showSection(sectionId) {
            // Hide all sections
            document.querySelectorAll('section').forEach(section => {
                section.classList.remove('visible');
            });
            // Show the selected section
            document.getElementById(sectionId).classList.add('visible');
        }
    </script>

</body>
</html>
