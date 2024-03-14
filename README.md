<!DOCTYPE html>
<html>
  <head>
    <title>...</title>
    <style>
      body {
        font-family: Arial, sans-serif;
        text-align: center;
        padding: 50px;
      }
    </style>
  </head>
  <body>
    <h1 id="message"></h1>

    <script>
      // Update the message every minute
      setInterval(function() {
        // Get the current time
        const now = new Date();
        const hours = now.getHours();
        const minutes = now.getMinutes();
        const seconds = now.getSeconds();

        // Check if it's 11:11
        if (hours === 11 && minutes === 11 && seconds === 0) {
          document.getElementById("message").innerText = "pide un deseo";
        } else {
          document.getElementById("message").innerText = "limon";
        }
      }, 60);
    </script>
  </body>
</html>
