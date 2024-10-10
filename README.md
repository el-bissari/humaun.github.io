<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My First Website</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-image: url('background.jpg');
            background-size: cover;
            background-position: center;
            margin: 0;
            padding: 0;
        }
        header {
            background-image: url('header-image.jpg');
            background-size: cover;
            color: white;
            text-align: center;
            padding: 2rem;
            height: 400px;
            position: relative;
        }
        header img {
            position: absolute;
            top: 20px;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 100px;
            border-radius: 50%;
            border: 2px solid white;
        }
        header h1 {
            margin-top: 120px;
            font-size: 2rem;
            text-shadow: 1px 1px 2px black;
        }
        .sliding-text {
            position: absolute;
            bottom: 10px;
            right: -100%;
            transform: translateY(0);
            background: rgba(255, 0, 0, 0.7);
            padding: 10px 20px;
            border-radius: 5px;
            white-space: nowrap;
            color: white;
            animation: slide 10s linear infinite;
            font-size: 1.5rem;
        }
        @keyframes slide {
            0% { right: -100%; }
            50% { right: 0; }
            100% { right: 100%; }
        }
        nav {
            background-color: rgba(68, 68, 68, 0.7);
            color: white;
            padding: 1rem;
            text-align: center;
        }
        nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
        }
        nav a:hover {
            text-decoration: underline;
            color: lightgray;
        }
        section {
            padding: 20px;
            margin: 20px;
            background-color: rgba(255, 255, 255, 0.8);
        }
        footer {
            text-align: center;
            padding: 10px;
            background-color: #333;
            color: white;
            position: fixed;
            bottom: 0;
            width: 100%;
        }

        /* বাটনের জন্য নতুন স্টাইলিং */
        button {
            background-color: #4CAF50;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            font-size: 1rem;
            cursor: pointer;
        }

        button:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>

    <header>
        <img src="long.png" alt="Website Logo">
        <h1>Welcome to My Website</h1>
        <div class="sliding-text">এটি একটি স্লাইডিং টেক্সট উদাহরণ।</div>
    </header>

    <nav>
        <a href="https://www.facebook.com/biplob8897">Home</a>
        <a href="#">About</a>
        <a href="#">Contact</a>
    </nav>

    <main>
        <section>
            <h2>About My Website</h2>
            <p>This is a simple webpage created using HTML and CSS. It contains a header, a navigation bar, a content section, and a footer.</p>
            <p>You can add more content here to make the website more informative. Consider including images, links, and other elements as needed.</p>

            <!-- নতুন বাটন যুক্ত করা হলো -->
            <button onclick="alert('Button clicked!')">Click Me</button>
        </section>
    </main>

    <footer>
        <p>&copy; 2024 My First Website</p>
    </footer>

</body>
</html>
