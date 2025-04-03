<!DOCTYPE html>
<html lang="zh-Hant">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>油漆／噴漆</title>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; padding: 20px; }
        .container { max-width: 600px; margin: auto; }
        img { width: 100%; max-width: 400px; margin-top: 20px; }
        .info { margin-top: 20px; }
        .contact { margin-top: 30px; font-weight: bold; }
    </style>
</head>
<body>
    <div class="container">
        <h2>高雄油漆0915189498</h2>
        <select id="techSelect">
            <option value="">-- 選擇技術 --</option>
            <option value="html">HTML</option>
            <option value="css">CSS</option>
            <option value="js">JavaScript</option>
        </select>
        <div class="info" id="info"></div>
        <div class="contact">聯絡方式：高雄油漆 洪重發油漆工程 0915189498</div>
    </div>
    <script>
        document.getElementById('techSelect').addEventListener('change', function() {
            var infoDiv = document.getElementById('info');
            var value = this.value;
            var content = "";
            
            if (value === "html") {
                content = "<img src='https://via.placeholder.com/400x200?text=HTML' alt='HTML'>" +
                          "<p>HTML（超文本標記語言）是建立網頁的基礎，用於結構化內容。</p>";
            } else if (value === "css") {
                content = "<img src='https://via.placeholder.com/400x200?text=CSS' alt='CSS'>" +
                          "<p>CSS（層疊樣式表）負責美化網頁，使其更具吸引力。</p>";
            } else if (value === "js") {
                content = "<img src='https://via.placeholder.com/400x200?text=JavaScript' alt='JavaScript'>" +
                          "<p>JavaScript 是用於讓網頁具有互動功能的程式語言。</p>";
            }
            infoDiv.innerHTML = content;
        });
    </script>
</body>
</html>
