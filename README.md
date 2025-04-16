<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>FakeTube</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f9f9f9;
      margin: 0;
      padding: 0;
    }
    header {
      background-color: #ff0000;
      color: white;
      padding: 15px;
      text-align: center;
    }
    #searchContainer {
      text-align: center;
      margin: 20px;
    }
    #searchInput {
      padding: 10px;
      width: 300px;
      font-size: 16px;
    }
    #searchButton {
      padding: 10px 20px;
      font-size: 16px;
      cursor: pointer;
    }
    .video-grid {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
      padding: 20px;
    }
    .video {
      width: 300px;
      background-color: white;
      border: 1px solid #ddd;
      border-radius: 10px;
      overflow: hidden;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }
    .video img {
      width: 100%;
    }
    .video h3 {
      margin: 10px;
    }
    footer {
      text-align: center;
      padding: 15px;
      background-color: #eee;
      margin-top: 50px;
    }
  </style>
</head>
<body>

  <header>
    <h1>FakeTube</h1>
  </header>

  <div id="searchContainer">
    <input id="searchInput" type="text" placeholder="Search..." />
    <button id="searchButton" onclick="search()">Search</button>
  </div>

  <div class="video-grid">
    <div class="video">
      <img src="https://i.ytimg.com/vi/pIJhWXJqX30/hqdefault.jpg" alt="Fergus Thumbnail" />
      <h3>Fergus being a sneaky cat 🐾</h3>
    </div>
    <div class="video">
      <img src="https://via.placeholder.com/300x180.png?text=Coming+Soon" alt="Placeholder" />
      <h3>More videos coming soon!</h3>
    </div>
  </div>

  <footer>
    &copy; 2025 FakeTube Inc.
  </footer>

  <script>
    function search() {
      const query = document.getElementById('searchInput').value.toLowerCase();
      if (query.includes('fergus')) {
        window.location.href = 'https://www.youtube.com/shorts/pIJhWXJqX30';
      } else {
        alert('No results found for "' + query + '". Try "fergus"!');
      }
    }
  </script>

</body>
</html>
