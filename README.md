# Basics Information about WEB-Technologies

## 1. Differences Between Previous HTML Versions and the Latest Version

### **What Changed from HTML4 to HTML5?**
- **HTML4** required **Flash** for videos, while **HTML5** introduced the `<video>` tag.
- **New Semantic Elements**: `<article>`, `<section>`, `<nav>` for better page structure.
- **Offline Capabilities**: HTML5 supports offline web apps using the **Cache API**.
- **Enhanced Forms**: New input types like `email`, `date`, `range`, and built-in validation.

### **Example:**
```html
<!-- HTML5 Video Support -->
<video controls>
    <source src="video.mp4" type="video/mp4">
</video>
```

---

## 2. How to Structure a Model in HTML?

### **What is HTML Structure?**
Think of an HTML page as a **house**:
- **Foundation** → `<html>`
- **Rooms** → `<header>`, `<section>`, `<footer>`
- **Doors & Windows** → `<nav>`, `<a>`, `<button>`

### **Example:**
```html
<!DOCTYPE html>
<html>
<head>
    <title>Website Structure</title>
</head>
<body>
    <header>Website Header</header>
    <nav>Navigation Menu</nav>
    <section>Main Content</section>
    <footer>Footer</footer>
</body>
</html>
```

---

## 3. What is CSS, and How Do CSS Frameworks Help?

### **CSS (Cascading Style Sheets)**
CSS is like **clothing** for HTML – it controls how a webpage looks.

### **CSS Frameworks (Bootstrap, Tailwind, etc.)**
- **Without Framework**: You style everything manually.
- **With Bootstrap**: Use prebuilt classes like `btn-primary` for styling.

### **Example (Using Bootstrap)**
```html
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css">
<button class="btn btn-primary">Click Me</button>
```

---

## 4. How is JavaScript Used for Functionality? What Libraries Like jQuery Are Used in Mobile Apps?

### **Why Use JavaScript?**
JS adds **interactivity** – clicking buttons, animations, form validation, etc.

### **jQuery – Simplifying JavaScript**
Instead of writing long JavaScript code, jQuery allows short and simple functions.

### **Example:**
```html
<button id="changeText">Click Me</button>
<p id="text">Hello!</p>

<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
<script>
    $("#changeText").click(function() {
        $("#text").text("Text Changed!");
    });
</script>
```

### **JavaScript Frameworks for Mobile Apps:**
- **React Native**
- **Ionic**
- **Flutter (supports JS integration)**

---

## 5. Where is JavaScript Used—Frontend or Backend?

### **Frontend (User Interaction)**
- Clicking buttons
- Form validation
- Animations

### **Backend (Using Node.js)**
- Handling databases
- User authentication
- API requests

---

## 6. Is PHP a Backend Language? Was Facebook Developed in PHP? What is Laravel?

- **PHP** is a backend scripting language.
- **Facebook** initially used PHP but later switched to **Hack (an evolved version of PHP)**.
- **Laravel** is a PHP framework that speeds up development.

### **Example – Simple PHP Login System**
```php
<?php
$users = ["admin" => "1234"];
$username = $_POST['username'];
$password = $_POST['password'];

if (isset($users[$username]) && $users[$username] === $password) {
    echo "Login Successful";
} else {
    echo "Login Failed";
}
?>
```

---

## 7. Difference Between Frontend and Backend Development

### **Example: A Restaurant**
- **Frontend (Waiter & Menu)** → What users see and interact with.
- **Backend (Kitchen & Chef)** → Where actual processing happens (database, server).

### **Technologies Used:**
| Category  | Technologies |
|-----------|-------------|
| Frontend  | HTML, CSS, JavaScript, React, Angular |
| Backend   | PHP, Node.js, Python, Java |

---

## 8. Difference Between Local and Online Databases

- **Local Database** → Like a personal diary on your desk (Example: SQLite).
- **Online Database** → Like Google Drive, accessible from anywhere (Example: MySQL, Firebase).

---

## 9. How is SQL Used in PHP for Storing Application Data?

### **SQL in PHP Example:**
```php
$conn = new mysqli("localhost", "root", "", "users_db");
$sql = "SELECT * FROM users";
$result = $conn->query($sql);
```

---

## 10. How is AJAX Used in jQuery?

### **Why Use AJAX?**
AJAX allows updating web pages **without refreshing**.

### **Example:**
```html
<button id="loadData">Load Data</button>
<div id="result"></div>

<script>
$("#loadData").click(function(){
    $.ajax({
        url: "data.txt",
        success: function(result){
            $("#result").html(result);
        }
    });
});
</script>
```

---

## 11. Differences Between Web 1.0, Web 2.0, and Web 3.0

| Feature   | Web 1.0 (Static) | Web 2.0 (Interactive) | Web 3.0 (Decentralized) |
|-----------|----------------|----------------------|----------------------|
| Interaction | Read-only | Social Media, Comments | AI, Blockchain |
| Examples  | Early Websites | Facebook, YouTube | Crypto, AI-based apps |

---

