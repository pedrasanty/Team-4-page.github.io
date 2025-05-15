<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Our Team</title>
<style>
  body {
    font-family: Arial, sans-serif;
    margin: 20px;
  }

  /* Navigation section fixed at the top right using position */
  nav {
    position: fixed;
    top: 20px;
    right: 20px;
    background: #333;
    padding: 10px 15px;
    border-radius: 5px;
  }
  nav a {
    color: white;
    text-decoration: none;
    margin-left: 15px;
    font-weight: bold;
  }
  nav a:hover {
    text-decoration: underline;
  }

  /* Container for all team members */
  .team-container {
    margin-top: 80px; /* space below fixed nav */
  }

  /* Each member's box */
  .team-member {
    width: 48%;
    margin-bottom: 30px;
    float: left;
    border: 1px solid #ccc;
    padding: 10px;
    box-sizing: border-box;
    border-radius: 8px;
    background: #f9f9f9;
  }

  /* Clear float after every two members */
  .team-member:nth-child(2n) {
    margin-right: 0;
  }

  /* Image styling */
  .team-member img {
    float: left;
    width: 120px;
    height: 120px;
    border-radius: 50%;
    margin-right: 15px;
  }

  /* Bio text */
  .bio {
    overflow: hidden; /* clears float inside */
  }

  /* Clear floats */
  .clearfix::after {
    content: "";
    display: table;
    clear: both;
  }
</style>
</head>
<body>

<nav>
  <a href="#">Home</a>
  <a href="#">Projects</a>
  <a href="#">Contact</a>
  <a href="#">About</a>
</nav>

<div class="team-container clearfix">

  <div class="team-member">
    <img src="https://randomuser.me/api/portraits/women/44.jpg" alt="Jane Doe" />
    <div class="bio">
      <h3>Jane Doe</h3>
      <p>Jane is our project manager with over 10 years experience in coordinating large teams and delivering quality results on time.</p>
    </div>
  </div>

  <div class="team-member">
    <img src="https://randomuser.me/api/portraits/men/36.jpg" alt="John Smith" />
    <div class="bio">
      <h3>John Smith</h3>
      <p>John is a software engineer specializing in frontend development. He loves creating intuitive user interfaces.</p>
    </div>
  </div>

  <div class="team-member">
    <img src="https://randomuser.me/api/portraits/women/68.jpg" alt="Lisa Wong" />
    <div class="bio">
      <h3>Lisa Wong</h3>
      <p>Lisa handles the marketing strategy and social media campaigns, helping grow our online presence globally.</p>
    </div>
  </div>

  <div class="team-member">
    <img src="https://randomuser.me/api/portraits/men/52.jpg" alt="Mark Johnson" />
    <div class="bio">
      <h3>Mark Johnson</h3>
      <p>Mark is our backend developer who ensures our servers and databases run smoothly and securely.</p>
    </div>
  </div>

</div>

</body>
</html>
