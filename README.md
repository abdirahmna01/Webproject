<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Web Design Company</title>
  <link rel="stylesheet" href="styl.css">
  <style>
    /* Internal CSS */
    :root {
      --primary-color: #2575fc;
      --secondary-color: #2575fc;
      --gradient: linear-gradient(45deg, var(--primary-color), var(--secondary-color));
      --text-color: #333;
      --white: #fff;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Poppins', sans-serif;
    }

    body {
      color: var(--text-color);
      line-height: 1.6;
      animation: fadeIn 1s ease-in;
    }

    @keyframes fadeIn {
      from {
        opacity: 0;
      }
      to {
        opacity: 1;
      }
    }

    /* Animation for sections */
    .body-section, .registration-section, footer {
      opacity: 0;
      transform: translateY(50px);
      animation: slideUp 1s ease-out forwards;
    }

    @keyframes slideUp {
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    /* Delays for section animations */
    .body-section {
      animation-delay: 0.5s;
    }

    .registration-section {
      animation-delay: 1s;
    }

    footer {
      animation-delay: 1.5s;
    }

    /* Header Section */
    header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 20px 10%;
      background: var(--gradient);
      color: var(--white);
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    }

    header .logo {
      font-size: 24px;
      font-weight: 600;
    }

    header nav {
      display: flex;
      align-items: center;
    }

    header nav a {
      color: var(--white);
      text-decoration: none;
      margin: 0 15px;
      font-weight: 500;
      transition: color 0.3s;
    }

    header nav a:hover {
      color: #ffdd40;
    }

    header .contact-btn {
      background: #ffdd40;
      color: var(--text-color);
      padding: 10px 20px;
      border-radius: 25px;
      text-decoration: none;
      font-weight: 600;
      transition: background 0.3s;
    }

    header .contact-btn:hover {
      background: #ffc107;
    }

    /* Body Section */
    .body-section {
      padding: 50px 10%;
    }

    .body-section .part {
      display: flex;
      align-items: center;
      margin-bottom: 50px;
    }

    .body-section .part img {
      width: 45%;
      border-radius: 15px;
    }

    .body-section .part .content {
      width: 50%;
      padding: 0 5%;
    }

    .body-section .part h1 {
      font-size: 36px;
      margin-bottom: 20px;
      color: var(--primary-color);
    }

    .body-section .part p {
      font-size: 18px;
      margin-bottom: 20px;
    }

    .body-section .part .btn {
      background: var(--gradient);
      color: var(--white);
      padding: 10px 20px;
      border-radius: 25px;
      text-decoration: none;
      font-weight: 600;
      transition: transform 0.3s;
    }

    .body-section .part .btn:hover {
      transform: scale(1.05);
    }

    /* Registration Section */
    .registration-section {
      padding: 50px 10%;
      background: var(--gradient);
      color: var(--white);
      text-align: center;
    }

    .registration-section h2 {
      font-size: 36px;
      margin-bottom: 20px;
    }

    .registration-section form {
      max-width: 500px;
      margin: 0 auto;
      display: flex;
      flex-direction: column;
      gap: 15px;
    }

    .registration-section input {
      padding: 10px;
      border-radius: 25px;
      border: none;
      outline: none;
      font-size: 16px;
    }

    .registration-section .submit-btn {
      background: #ffdd40;
      color: var(--text-color);
      padding: 10px 20px;
      border-radius: 25px;
      border: none;
      font-size: 16px;
      font-weight: 600;
      cursor: pointer;
      transition: background 0.3s;
    }

    .registration-section .submit-btn:hover {
      background: #ffc107;
    }

    /* Footer Section */
    footer {
      background: var(--gradient);
      color: var(--white);
      padding: 50px 10%;
      display: flex;
      justify-content: space-between;
      flex-wrap: wrap;
    }

    footer .footer-section {
      width: 23%;
    }

    footer .footer-section h3 {
      margin-bottom: 20px;
      font-size: 20px;
    }

    footer .footer-section a {
      display: block;
      color: var(--white);
      text-decoration: none;
      margin-bottom: 10px;
      transition: color 0.3s;
    }

    footer .footer-section a:hover {
      color: #ffdd40;
    }

    footer .copyright {
      width: 100%;
      text-align: center;
      margin-top: 30px;
      font-size: 14px;
    }

    /* Responsive Design */
    @media (max-width: 768px) {
      header {
        flex-direction: column;
        text-align: center;
      }

      header nav {
        margin-top: 15px;
      }

      .body-section .part {
        flex-direction: column;
      }

      .body-section .part img,
      .body-section .part .content {
        width: 100%;
        text-align: center;
      }

      footer .footer-section {
        width: 48%;
        margin-bottom: 30px;
      }
    }

    @media (max-width: 480px) {
      footer .footer-section {
        width: 100%;
      }
    }
  </style>
</head>
<body>
  <!-- Header Section -->
  <header>
    <div class="logo">Abdirahman</div>
    <nav>
      <a href="#home">Home</a>
      <a href="#About">About</a>
      <a href="#Regester">Regester</a>
      <a href="#contact" class="contact-btn">Contact</a>
    </nav>
  </header>

  <!-- Body Section -->
  <div class="body-section">
    <!-- Part 1 -->
    <div class="part">
      <div class="content">
        <h1>Welcome to Our Web Design Company</h1>
        <p>We specialize in creating stunning, responsive websites that help businesses grow. Let us bring your vision to life!</p>
        <a href="rtx.png" class="btn">Contact Us</a>
      </div>
      <img src="rtx.png" alt="Web Design">
    </div>

    <!-- Part 2 -->
    <div class="part">
      <img src="work.png" alt="Achievements">
      <div class="content">
        <h1>What Can You Achieve With Your Company Website?</h1>
        <p>From increased visibility to higher customer engagement, a well-designed website can transform your business.</p>
      </div>
    </div>
  </div>

  <!-- Registration Section -->
  <div class="registration-section">
    <h2>Register Now</h2>
    <form action="#" method="POST">
      <input type="text" name="firstName" placeholder="First Name" required>
      <input type="text" name="lastName" placeholder="Last Name" required>
      <input type="email" name="email" placeholder="Email" required>
      <button type="submit" class="submit-btn">Submit</button>
    </form>
  </div>

  <!-- Footer Section -->
  <footer>
    <div class="footer-section">
      <h3>Services</h3>
      <a href="#">Home</a>
      <a href="#">about</a>
      <a href="#">regester 3</a>
    </div>
    <div class="footer-section">
      <h3>Company</h3>
      <a href="#">Services</a>
      <a href="#">Locations</a>
      <a href="#">About</a>
    </div>
    <div class="footer-section">
      <h3>Global</h3>
      <a href="#">Privacy Policy</a>
      <a href="#">Terms of Service</a>
    </div>
    <div class="footer-section">
      <h3>Upcoming</h3>
      <a href="#">Your Company 2</a>
    </div>
    <div class="copyright">
      Copyright © 2024 Your Company. All Rights Reserved.
    </div>
  </footer>

  <!-- Internal JavaScript -->
  <script>
    // Add any interactive JavaScript here
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
      anchor.addEventListener('click', function (e) {
        e.preventDefault();
        document.querySelector(this.getAttribute('href')).scrollIntoView({
          behavior: 'smooth'
        });
      });
    });
  </script>
</body>
</html>

