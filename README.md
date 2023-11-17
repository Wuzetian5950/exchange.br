<!DOCTYPE html>

<html>
  <head>
    <title>Hell</title>
    <style>
        body {
            font-family: Arial, sans-serif;
        }
        .dropdown {
            position: relative;
            display: inline-block;
        }
        .dropdown-content {
            display: none;
            position: absolute;
            background-color: #f9f9f9;
            min-width: 160px;
            box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
            padding: 12px 16px;
            z-index: 1;
        }
        .dropdown:hover .dropdown-content {
            display: block;
        }
    </style>
</head>
<body>
    <h1>JavaScript Features</h1>
    <div class="dropdown">
        <button>Hover over me</button>
        <div class="dropdown-content">
            <p>Hello World!</p>
        </div>
    </div>

    <h2>JavaScript Alert</h2>
    <button onclick="displayAlert()">Click me</button>

    <h2>JavaScript Date</h2>
    <p id="date"></p>

    <script>
        function displayAlert() {
            alert("Hello, this is a JavaScript Alert!");
        }

        document.getElementById("date").innerHTML = "Today's date is " + new Date().toDateString();
    </script>
</body>
</html> 
