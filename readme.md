<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>초대장</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f3f3f3;
            margin: 0;
        }
        .container {
            position: relative;
            cursor: pointer;
            display: inline-block;
        }
        .container img {
        width: 100%; /* 추가 */
        height: auto; /* 추가 */
        }
        .message {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.7);
            color: white;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 18px;
            font-weight: bold;
            display: none;
        }
    </style>
</head>
<body>
    <div class="container" onclick="handleClick()">
        <img id="invitation" src="https://github.com/yoon-zip/SEF2025/blob/main/invitation2.png?raw=true" alt="초대장" width="300">
        <div id="message" class="message">클릭하면 신청 페이지로 이동합니다.</div>
    </div>
    
    <script>
        function handleClick() {
            window.location.href = "https://naver.me/FuzdiiHA"; // 네이버폼 링크로 이동
        }
    </script>
</body>
</html>
