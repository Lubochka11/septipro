<!DOCTYPE html>  
<html lang="ru">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0">  
    <title>Доступ ограничен</title>  
    <style>  
        * { margin: 0; padding: 0; box-sizing: border-box; }  
        body {  
            font-family: -apple-system, sans-serif;  
            background: #f5f5f5;  
            display: flex;  
            justify-content: center;  
            align-items: center;  
            height: 100vh;  
        }  
        .lock-box {  
            background: #fff;  
            padding: 40px;  
            border-radius: 12px;  
            text-align: center;  
            box-shadow: 0 2px 16px rgba(0,0,0,0.08);  
            max-width: 400px;  
            width: 100%;  
        }  
        .lock-icon { font-size: 48px; margin-bottom: 16px; }  
        h1 { font-size: 22px; margin-bottom: 8px; }  
        p { color: #888; margin-bottom: 24px; }  
        input {  
            width: 100%;  
            padding: 12px;  
            border: 1px solid #ddd;  
            border-radius: 8px;  
            font-size: 16px;  
            margin-bottom: 12px;  
            text-align: center;  
        }  
        button {  
            width: 100%;  
            padding: 12px;  
            background: #4caf50;  
            color: #fff;  
            border: none;  
            border-radius: 8px;  
            font-size: 16px;  
            cursor: pointer;  
        }  
        button:hover { background: #43a047; }  
        .error { color: #e53935; font-size: 14px; margin-top: 8px; display: none; }  
    </style>  
</head>  
<body>  
<div class="lock-box">  
    <div class="lock-icon">🔒</div>  
    <h1>Сайт в разработке</h1>  
    <p>Введите пароль для доступа</p>  
    <input type="password" id="passInput" placeholder="Пароль">  
    <button onclick="checkPass()">Войти</button>  
    <p class="error" id="error">Неверный пароль</p>  
</div>  
<script>  
    function checkPass() {  
        var p = document.getElementById('passInput').value;  
        if (p === 'test2026') {  
            window.location.href = '/catalog.html';  
        } else {  
            document.getElementById('error').style.display = 'block';  
        }  
    }  
</script>  
</body>  
</html>  
