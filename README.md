# Learnify

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Learnify - Home</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="sidebar">
        <h2>Learnify</h2>
        <a href="index.html" class="active">🏠 Home</a>
        
        <div class="dropdown">
            <button class="dropdown-btn">📘 Math ▾</button>
            <div class="dropdown-content">
                <a href="subjects/math.html">Go to Math</a>
            </div>
        </div>

        <div class="dropdown">
            <button class="dropdown-btn">🔬 Science ▾</button>
            <div class="dropdown-content">
                <a href="subjects/science.html">Go to Science</a>
            </div>
        </div>

        <div class="dropdown">
            <button class="dropdown-btn">📖 English ▾</button>
            <div class="dropdown-content">
                <a href="subjects/english.html">Go to English</a>
            </div>
        </div>

        <div class="dropdown">
            <button class="dropdown-btn">💻 Coding ▾</button>
            <div class="dropdown-content">
                <a href="subjects/coding.html">Go to Coding</a>
            </div>
        </div>
    </div>

    <div class="content">
        <h1>Welcome to Learnify</h1>
        <p>Select a subject to begin learning.</p>

        <div class="subjects-grid">
            <a href="subjects/math.html" class="subject-card">📘 Math</a>
            <a href="subjects/science.html" class="subject-card">🔬 Science</a>
            <a href="subjects/english.html" class="subject-card">📖 English</a>
            <a href="subjects/coding.html" class="subject-card">💻 Coding</a>
        </div>
    </div>
</body>
</html>

/* General Styling */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    display: flex;
}

/* Sidebar Navigation */
.sidebar {
    width: 250px;
    background: #333;
    color: white;
    height: 100vh;
    position: fixed;
    padding-top: 20px;
}

.sidebar h2 {
    text-align: center;
}

.sidebar a, .dropdown-btn {
    display: block;
    color: white;
    padding: 15px;
    text-decoration: none;
    background: none;
    border: none;
    width: 100%;
    text-align: left;
    cursor: pointer;
    font-size: 16px;
}

.sidebar a:hover, .dropdown-btn:hover {
    background: #007bff;
}

/* Dropdown (Parent-Child Navigation) */
.dropdown-content {
    display: none;
    background: #444;
}

.dropdown:hover .dropdown-content {
    display: block;
}

/* Content Area */
.content {
    margin-left: 250px;
    padding: 20px;
    flex-grow: 1;
}

/* Subjects Grid (Homepage) */
.subjects-grid {
    display: flex;
    gap: 20px;
    flex-wrap: wrap;
}

.subject-card {
    background: white;
    padding: 20px;
    text-align: center;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    text-decoration: none;
    color: black;
    font-size: 18px;
}

.subject-card:hover {
    background: #007bff;
    color: white;
}
