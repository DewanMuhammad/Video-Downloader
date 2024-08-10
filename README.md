<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Video Downloader</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
        }
        .container {
            max-width: 600px;
            margin: auto;
            text-align: center;
        }
        input[type="text"] {
            width: 80%;
            padding: 10px;
            margin-bottom: 10px;
            font-size: 16px;
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
        }
        .status {
            margin-top: 20px;
        }
    </style>
</head>
<body>

<div class="container">
    <h2>Video Downloader</h2>
    <form id="downloadForm" action="download.php" method="post">
        <input type="text" id="videoUrl" name="videoUrl" placeholder="Enter video URL" required>
        <button type="submit">Download Video</button>
    </form>
    <p class="status"><?php if(isset($_GET['status'])) { echo $_GET['status']; } ?></p>
</div>

</body>
</html>
# Video-Downloader
