- 👋 Hi, I’m Barshan Patar
- 👀 I’m interested in Web Devolopment
- 🌱 I’m currently learning the basic of web devolopment (HTML,CSS,JS)
- 💞️ I’m looking to collaborate on Project usnig the basic of web devolopment.
- 📫 How to reach me-
- Call/Whatsapp- 7319546936
- email- barshan8348@gmail.com
- 

<!---
Barshan Patar is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<!DOCTYPE html>
<html>
<head>
  <title>Left Panel Example</title>
  <style>
    /* General styling */
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
    }

    /* Styling for the left panel */
    #left-panel {
      width: 200px;
      height: 100%;
      background: #f2f2f2;
      float: left;
    }

    #left-panel ul {
      list-style-type: none;
      margin: 0;
      padding: 0;
    }

    #left-panel li {
      margin-bottom: 10px;
    }

    #left-panel li a {
      display: block;
      padding: 10px;
      color: #333;
      text-decoration: none;
      transition: background-color 0.3s ease;
    }

    #left-panel li a:hover {
      background-color: #ccc;
    }

    /* Styling for the content area */
    #content {
      padding: 20px;
    }

    #content h2 {
      color: #333;
    }

    #content p {
      color: #666;
    }

    /* Responsive styles */
    @media screen and (max-width: 768px) {
      #left-panel {
        width: 100%;
        height: auto;
        float: none;
      }

      #content {
        margin-left: 0;
      }
    }
  </style>
  <script>
    // JavaScript code to handle component clicks and show corresponding content
    function showContent(component) {
      var contentDiv = document.getElementById('content');
      
      // Clear existing content
      contentDiv.innerHTML = '';
      
      // Add new content based on the selected component
      if (component === 'home') {
        contentDiv.innerHTML = '<h2>Welcome to the Home Page!</h2><p>This is the home page content.</p>';
      } else if (component === 'contact') {
        contentDiv.innerHTML = '<h2>Contact Information</h2><p>Here is our contact information.</p>';
      } else if (component === 'information') {
        contentDiv.innerHTML = '<h2>Information</h2><p>Here is some information for you.</p>';
      } else if (component === 'guide') {
        contentDiv.innerHTML = '<h2>Guide</h2><p>Here is a helpful guide for you.</p>';
      }
    }
  </script>
</head>
<body>
  <div id="left-panel">
    <!-- Left panel navigation -->
    <ul>
      <li><a href="#" onclick="showContent('home')">Home</a></li>
      <li><a href="#" onclick="showContent('contact')">Contact</a></li>
      <li><a href="#" onclick="showContent('information')">Information</a></li>
      <li><a href="#" onclick="showContent('guide')">Guide</a></li>
    </ul>
  </div>
  <div id="content">
    <!-- Content area -->
    <h2>Welcome to the Home Page!</h2>
    <p>This is the initial content.</p>
  </div>
</body>
</html>