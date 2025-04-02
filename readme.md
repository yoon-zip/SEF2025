<!DOCTYPE html>
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
    <div class="container">
        <img id="invitation" src="https://raw.githubusercontent.com/yoon-zip/SEF2025/refs/heads/main/invitaion.png" alt="초대장" width="300">
        <div id="message" class="message">클릭하면 신청 페이지로 이동합니다.</div>
    </div>

    <script>
        let clicked = false;
        document.getElementById('invitation').addEventListener('click', function() {
            if (!clicked) {
                document.getElementById('message').style.display = 'flex';
                clicked = true;
            } else {
                window.location.href = "https://naver.me/FuzdiiHA"; // 네이버폼 링크
            }
        });
    </script>
</body>
</html>
