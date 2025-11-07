<html>
<meta charset="UTF-8">
<title>Flaraa</title>
<meta name="viewport" content="width=device-width,initial-scale=1">
<link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
<link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" rel="stylesheet">
<style>
body {font-family: 'Brush Script MT', cursive;}
h1,h2,h3,h4,h5,h6 {font-family: 'Brush Script MT', cursive; letter-spacing:5px}

.counter {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background: #fff;
      color: #333;
      padding: 10px 20px;
      border-radius: 50px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
      font-size: 1.2rem;
      display: flex;
      align-items: center;
      justify-content: center;
      animation: bounce 1s infinite;
    }
    .counter i {
      margin-right: 5px;
      color: #ff7e5f;
    }
    /* Animations */
    @keyframes fadeIn {
      0% { opacity: 0; }
      100% { opacity: 1; }
    }
    @keyframes slideUp {
      0% { transform: translateY(20px); opacity: 0; }
      100% { transform: translateY(0); opacity: 1; }
    }
    @keyframes bounce {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-10px); }
    }


</style>
<body>

<!-- Navigation (Sits on top) -->
<div class="w3-top w3-bar w3-white w3-padding w3-card w3-wide">
<a href="#home" class="w3-bar-item w3-button" style="font-size: 48px; color: #8E403A; font-family: 'Brush Script MT', cursive;">FLARAA</a>

<!-- Right-sided navbar links. Hide them on small screens -->

</div>

<!-- Start Content -->
<div id="home" class="w3-content">

<!-- Image in Display Container -->
<div class="w3-padding-top-48">
<div class="w3-display-container">
<br><img src="group.jpg" alt="Catering" style="width:100%; height: 300px;">

<div class="w3-display-bottomleft w3-padding-small w3-opacity w3-hide-small">
<h2>---</h2>
</div>

</div>
</div>
<h5 style="font-size: 28px;" class="w3-center">Innovating since Nov 2024</h5>
<!-- About -->
<div id="about" class="w3-padding-top-64">
<div class="w3-row">

<div class="w3-col l6 m6 w3-padding-large">
<img src="profile1.jpg" class="w3-round w3-image w3-opacity-min" alt="Table" style="width:100%">
</div>

<div class="w3-half w3-padding-large">
<h1 class="w3-center">Profile</h1>
<p class="w3-large" style="font-family: 'Brush Script MT', cursive;">
Our platform is a social media website where individuals can create personalized profiles. Connect, discover, and explore others’ profiles in a community built for self-expression and meaningful interactions.</p>

</div>

</div>
</div>

<div id="about" class="w3-padding-top-64">
<div class="w3-row">

<div class="w3-col l6 m6 w3-padding-large">
<img src="texting.jpg" class="w3-round w3-image w3-opacity-min" alt="Table" style="width:100%">
</div>

<div class="w3-half w3-padding-large">
<h1 class="w3-center">Messaging</h1>
<p class="w3-large" style="font-family: 'Brush Script MT', cursive;">
Our social media platform enables individuals to connect instantly through seamless text messaging. Stay in touch with friends, family, and new connections with real-time chats, private conversations, and group messaging. Share thoughts, updates, and moments effortlessly in a secure and user-friendly environment.</p>

</div>

</div>
</div>


<div id="menu" class="w3-padding-top-64">
<h1 class="w3-center">Safety & Security</h1>
<div class="w3-row">

<div class="w3-col l6 m6 w3-padding-large">

<h4>General</h4>
<span class="w3-text-grey">
Options like restricted, hide, block and selected user visibility is available.
Selected user visibility means users can select who can view their profile like .edu or @company.com or everyone</span><br><br>

<h4>Secured Login</h4>
<span class="w3-text-grey">
Password hashing is provided to protect users' data from data theft.</span><br><br>

<h4>SQL Injection</h4>
<span class="w3-text-grey">
Implemented with securities to ensure data integrity and prevent SQL injection attacks when handling database queries.</span><br><br>

<h4>Report and Issue</h4>
<span class="w3-text-grey">
We will provide “Report an issue” section to prevent security threats.</span>
</div>

<div class="w3-col l6 m6 w3-padding-large">
<img src="safety.jpg" class="w3-round w3-image w3-opacity-min" alt="Menu" style="width:100%">
</div>

</div>
</div>

<div id="about_us" class="w3-padding-top-64">
<h1 class="w3-center">About Us</h1>
<div class="w3-row">

<div class="w3-col l6 m6 w3-padding-large">

<span style="font-size: 20px">Shweta M. K.</span><br>
<span class="w3-text-grey">
First Semester <br> MS in Computer Engineering, SJSU</span><br><br>
</div>

<div class="w3-col l6 m6 w3-padding-large">
<img src="about_us.jpg" class="w3-round w3-image w3-opacity-min" alt="Menu" style="width:100%">
</div>

</div>
</div>

<div id="contact" class="w3-container w3-padding-64">
<h1>Contact</h1>

<p class="w3-text-blue-grey w3-large">
<b>One Washington Square, San Jose, CA, 95192</b></p>
<p>You can also contact me by email shwethha10@gmail.com</p>

<img src="map.jpg" class="w3-image" style="width:100%; height: 300px">
</div> 


<div class="counter" id="visitCount">
    <i class="fas fa-eye"></i> Loading...
  </div>

  <script>
    (function() {
      const domain = encodeURIComponent(window.location.hostname);
      const timezone = Intl.DateTimeFormat().resolvedOptions().timeZone;
      const page_path = window.location.pathname;
      const page_title = document.title;
      const referrer = document.referrer;

      fetch('https://visitor.6developer.com/visit', {
        method: 'POST',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify({
          domain,
          timezone,
          page_path,
          page_title,
          referrer
        })
      })
      .then(response => response.json())
      .then(data => {
        document.getElementById("visitCount").innerHTML = `<i class="fas fa-eye"></i> ${data.totalCount}`;
      })
      .catch(error => {
        console.error('Error:', error);
        document.getElementById("visitCount").innerHTML = `<i class="fas fa-eye"></i> Error`;
      });
    })();
  </script>

