<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Free Proxy</title>
</head>
<body>
    <h1>Free Proxy Website</h1>
    <form action="proxy.php" method="get">
        <label for="url">Enter a URL:</label>
        <input type="text" name="url" id="url" placeholder="http://example.com" required>
        <button type="submit">Go</button>
    </form>
</body>
</html>
<?php
if (isset($_GET['url'])) {
    $url = $_GET['url'];
    echo file_get_contents($url);
}
?>
