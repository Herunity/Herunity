<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>HerUnity Network</title>

  <!-- Google Fonts for a beautiful font -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@600&display=swap" rel="stylesheet">

  <style>
    body {
      font-family: 'Poppins', sans-serif; /* Beautiful, elegant font */
      margin: 0;
      padding: 0;
      background-color: #f8f0ff; /* Very light purple */
      color: #333;
    }
    header {
      background-color: #6a1b9a; /* Dark purple */
      color: #fff;
      padding: 20px;
      text-align: center;
    }
    header h1 {
      margin: 0;
    }
    header h1 strong {
      font-weight: bold; /* Make only "Her" bold */
    }
    nav {
      background-color: #8e44ad; /* Medium purple */
      padding: 10px;
      text-align: center;
    }
    nav a {
      color: #fff;
      text-decoration: none;
      margin: 0 15px;
      font-weight: bold;
    }
    nav a:hover {
      text-decoration: underline;
    }
    section {
      padding: 20px;
      max-width: 1200px;
      margin: auto;
    }
    .program {
      background: #f3e5f5; /* Light purple for program cards */
      border: 1px solid #8e44ad; /* Medium purple */
      border-radius: 8px;
      padding: 15px;
      margin: 15px 0;
    }
    .program h3 {
      color: #6a1b9a; /* Dark purple */
      margin-bottom: 10px;
    }
    .program p {
      margin: 5px 0;
    }
    footer {
      background-color: #8e44ad; /* Medium purple */
      color: #fff;
      text-align: center;
      padding: 10px;
      position: fixed;
      bottom: 0;
      width: 100%;
    }

    /* Sponsors Section */
    .sponsors {
      background-color: #ffffff;
      padding: 20px;
      text-align: center;
      margin-top: 40px;
    }
    .sponsors h2 {
      color: #6a1b9a; /* Dark purple */
      margin-bottom: 20px;
    }
    .sponsors img {
      max-width: 200px;
      margin: 0 20px;
      border-radius: 8px;
    }

    /* Popup Styles */
    .popup {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(106, 27, 154, 0.5); /* Semi-transparent dark purple overlay */
      display: flex;
      justify-content: center;
      align-items: center;
      visibility: hidden;
      opacity: 0;
      transition: opacity 0.3s, visibility 0.3s;
    }
    .popup.show {
      visibility: visible;
      opacity: 1;
    }
    .popup-content {
      background: #fff;
      padding: 20px;
      border-radius: 10px;
      text-align: center;
      box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.2);
      max-width: 400px;
      width: 90%;
    }
    .popup-content h3 {
      color: #6a1b9a; /* Dark purple */
      margin-bottom: 10px;
    }
    .popup-content p {
      margin-bottom: 20px;
      color: #555;
    }
    .popup-content button {
      padding: 15px 30px;
      background-color: #8e44ad; /* Medium purple */
      color: #fff;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      font-weight: bold;
      font-size: 18px;
      text-transform: uppercase;
    }
    .popup-content button:hover {
      background-color: #6a1b9a; /* Dark purple */
    }
  </style>
</head>
<body>
  <header>
    <h1><strong>Her</strong>Unity Network</h1>
    <p>Empowering young women to lead in business and finance.</p>
  </header>
  <nav>
    <a href="#about">About Us</a>
    <a href="#programs">Programs</a>
    <a href="#get-involved">Get Involved</a>
    <a href="#contact">Contact</a>
  </nav>
  <section id="about">
    <h2>About Us</h2>
    <p>The HerUnity Network is dedicated to empowering young women in high school and early university stages to thrive in business, finance, and leadership roles. Through my own experiences growing up, I have learned that it’s crucial to encourage young girls to actively participate in extracurricular activities in competitive environments. I want to help them believe that they belong in the rooms they aspire to be in, giving them the confidence they need to succeed and excel in their chosen fields.</p>
  </section>
  <section id="programs">
    <h2>Our Programs</h2>
    <!-- Example Program -->
    <div class="program">
      <h3>Skill-Building Workshops</h3>
      <p>Interactive workshops on financial literacy, business basics, and leadership development.</p>
    </div>
  </section>
  
  <!-- Sponsors Section -->
  <section id="sponsors" class="sponsors">
    <h2>Our Sponsors</h2>
    <p>We are grateful for the generous support of our sponsors who help us make a difference.</p>
    <!-- Sponsor Logo Example -->
    <img src="https://via.placeholder.com/200x100?text=Sponsor+Logo" alt="Sponsor Logo">
  </section>

  <footer>
    <p>&copy; 2024 HerUnity Network. All Rights Reserved.</p>
  </footer>

  <!-- Popup Structure -->
  <div id="popup" class="popup">
    <div class="popup-content">
      <h3>How to Contribute</h3>
      <p>You can support HerUnity Network by volunteering, mentoring, donating, or sharing our mission with others.</p>
      <button id="closePopup">Got It</button>
    </div>
  </div>

  <script>
    // JavaScript for Popup
    document.addEventListener("DOMContentLoaded", function () {
      const popup = document.getElementById("popup");
      const closePopupButton = document.getElementById("closePopup");

      // Show the popup when the page loads
      setTimeout(() => {
        popup.classList.add("show");
      }, 1000); // Delay of 1 second

      // Close the popup when the button is clicked
      closePopupButton.addEventListener("click", function () {
        popup.classList.remove("show");
      });
    });
  </script>
</body>
</html>

