<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tech Site</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Tech Site</h1>
        <button id="theme-toggle">Toggle Dark Mode</button>
    </header>
    <main>
        <section id="content">
            <h2>Latest Tech News</h2>
            <p>Here you can add your tech news content...</p>
        </section>
    </main>
    <script src="script.js"></script>
</body>
</html>
styles.css:

body {
    font-family: Arial, sans-serif;
    background-color: white;
    color: black;
    transition: background-color 0.3s, color 0.3s;
}

body.dark-mode {
    background-color: #121212;
    color: white;
}

header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem;
    background-color: #f8f9fa;
}

header.dark-mode {
    background-color: #1f1f1f;
}

button {
    padding: 0.5rem 1rem;
    cursor: pointer;
}
script.js:

document.getElementById('theme-toggle').addEventListener('click', () => {
    document.body.classList.toggle('dark-mode');
    document.querySelector('header').classList.toggle('dark-mode');
});
