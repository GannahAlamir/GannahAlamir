
<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bahy Store</title>
    <link rel="stylesheet" href="styles.css">
    <link rel="stylesheet" href="style.css">
    
</head>
<body>
    <header>
        <nav>
            <h1>Bahy Store</h1>
            <ul>
                <li><a href="#home">الرئيسية</a></li>
                <li><a href="#about">من نحن</a></li>
                <li><a href="#services">خدماتنا</a></li>
                <li><a href="#contact">اتصل بنا</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section id="home">
            <h2>مرحبًا بكم في Bahy Store</h2>
            <p>أفضل خدمات الدعاية والإعلان.</p>
        </section>
        <section id="about">
            <h2>من نحن</h2>
            <p>نحن شركة متخصصة في خدمات الدعاية والإعلان.</p>
        </section>
        <section id="services">
            <h2>خدماتنا</h2>
            <ul>
                <li>تصميم الجرافيك</li>
                <li>إدارة الحملات الإعلانية</li>
                <li>التسويق الرقمي</li>
            </ul>
        </section>
        <section id="contact">
            <h2>اتصل بنا</h2>
            <form>
                <label for="name">الاسم:</label>
                <input type="text" id="name" name="name" required>
                <label for="email">البريد الإلكتروني:</label>
                <input type="email" id="email" name="email" required>
                <label for="message">رسالتك:</label>
                <textarea id="message" name="message" required></textarea>
                <button type="submit">إرسال</button>
            </form>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 Bahy Store. جميع الحقوق محفوظة.</p>
    </footer>
    <script src="script.js"></script>
</body>
</html>

body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

header {
    background-color: #333;
    color: white;
    padding: 10px 0;
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 1200px;
    margin: auto;
    padding: 0 20px;
}

nav h1 {
    margin: 0;
}

nav ul {
    list-style: none;
    padding: 0;
    display: flex;
    gap: 20px;
}

nav ul li {
    display: inline;
}

nav ul li a {
    color: white;
    text-decoration: none;
    padding: 5px 10px;
    transition: background 0.3s;
}

nav ul li a:hover {
    background-color: #555;
}

main {
    max-width: 1200px;
    margin: 20px auto;
    padding: 0 20px;
}

section {
    margin-bottom: 40px;
}

h2 {
    color: #333;
}

ul {
    list-style: none;
    padding: 0;
}

form {
    display: flex;
    flex-direction: column;
    gap: 10px;
}

input, textarea, button {
    padding: 10px;
    font-size: 16px;
}

button {
    background-color: #333;
    color: white;
    border: none;
    cursor: pointer;
    transition: background 0.3s;
}

button:hover {
    background-color: #555;
}

footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 10px 0;
}
 // script.js

 document.addEventListener("DOMContentLoaded", function() {
    const form = document.querySelector("form");
    form.addEventListener("submit", function(event) {
        event.preventDefault();
        alert("تم إرسال رسالتك بنجاح!");
        form.reset();
    });
});
