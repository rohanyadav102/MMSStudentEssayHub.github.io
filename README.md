<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Student Essay Hub</title>
    <link rel="stylesheet" href="styles.css">
    <style>
        /* Basic CSS for demonstration purposes */
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
        }
        header {
            background: #333;
            color: #fff;
            padding: 10px 0;
            text-align: center;
        }
        .hero {
            background: url(data:image/jpeg;base64,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) no-repeat center center/cover;
            color: #fff;
            padding: 100px 20px;
            text-align: center;
        }
        .hero h1 {
            font-size: 3em;
        }
        .hero p {
            font-size: 1.5em;
        }
        .btn {
            background: #007BFF;
            color: #fff;
            padding: 10px 20px;
            text-decoration: none;
            border-radius: 5px;
        }
        .section {
            padding: 20px;
            text-align: center;
        }
        .section img {
            width: 100%;
            max-width: 300px;
            height: auto;
        }
        footer {
            background: #333;
            color: #fff;
            padding: 10px 0;
            text-align: center;
        }
        .form-group {
            margin: 10px 0;
        }
    </style>
</head>
<body>

<header>
    <div class="container">
        <h1>Student Essay Hub</h1>
        <nav>
            <a href="#">Home</a> |
            <a href="#">About Us</a> |
            <a href="#">Essay Topics</a> |
            <a href="#">Submit Your Essay</a> |
            <a href="#">Contact Us</a>
        </nav>
    </div>
</header>

<div class="hero">
    <h1>Welcome to Student Essay Hub!</h1>
    <p>Explore Essays on Various Topics and Enhance Your Knowledge</p>
    <a href="#" class="btn">Get Started</a>
</div>

<div class="section">
    <h2>Featured Essays</h2>
    <div>
        <img src="essay1.jpg" alt="Essay 1">
        <h3>The Importance of Education in Our Country</h3>
        <p>Education is the cornerstone of a developed society...</p>
        <a href="#" class="btn">Read More</a>
    </div>
    <!-- Add more featured essays similarly -->
</div>

<div class="section">
    <h2>Submit Your Essay</h2>
    <form>
        <div class="form-group">
            <label for="name">Name</label>
            <input type="text" id="name" name="name" required>
        </div>
        <div class="form-group">
            <label for="email">Email</label>
            <input type="email" id="email" name="email" required>
        </div>
        <div class="form-group">
            <label for="title">Essay Title</label>
            <input type="text" id="title" name="title" required>
        </div>
        <div class="form-group">
            <label for="content">Essay Content</label>
            <textarea id="content" name="content" rows="5" required></textarea>
        </div>
        <div class="form-group">
            <label for="file">Upload Your Essay (optional)</label>
            <input type="file" id="file" name="file">
        </div>
        <button type="submit" class="btn">Submit</button>
    </form>
</div>

<footer>
    <p>© 2024 Student Essay Hub. All rights reserved.</p>
    <p>
        <a href="#">Home</a> |
        <a href="#">About Us</a> |
        <a href="#">Essay Topics</a> |
        <a href="#">Submit Your Essay</a> |
        <a href="#">Contact Us</a>
    </p>
</footer>

</body>
</html>
