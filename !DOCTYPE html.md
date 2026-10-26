<!DOCTYPE html>  
<html lang="ar" dir="rtl">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0">  
    <title>Love Message</title>  
    <style>  
        body {  
            background-color: #f7f2ed;  
            font-family: Tahoma, sans-serif;  
            display: flex;  
            justify-content: center;  
            align-items: center;  
            height: 100vh;  
            margin: 0;  
            text-align: center;  
        }  
        .container {  
            background: white;  
            padding: 30px;  
            border-radius: 20px;  
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);  
            max-width: 350px;  
            width: 90%;  
        }  
        h2 { color: #d9534f; }  
        input {  
            padding: 10px;  
            width: 80%;  
            border: 1px solid #ddd;  
            border-radius: 10px;  
            margin: 15px 0;  
            text-align: center;  
            font-size: 16px;  
        }  
        button {  
            background-color: #d9534f;  
            color: white;  
            border: none;  
            padding: 10px 20px;  
            border-radius: 10px;  
            cursor: pointer;  
            font-size: 16px;  
        }  
        .hidden { display: none; }  
    </style>  
</head>  
<body>  
  
<div class="container" id="lock-screen">  
    <h2>🔒 أُدخل كلمة السر</h2>  
    <p>هذه الهدية مخصصة لك وحدك</p>  
    <input type="password" id="passcode" placeholder="اكتب كلمة السر...">  
    <br>  
    <button onclick="checkPassword()">فتح الرسالة</button>  
</div>  
  
<div class="container hidden" id="message-screen">  
    <h2>my everything ❤️</h2>  
    <p>حبيت أعمل هدية بسيطة ومميزة لك، وأقولك قد إيش أنا بحبك، ربنا يخليك لي يا قلبي ولا يحرمني منك أبداً!</p>  
    <p style="font-size: 24px;">💍✨</p>  
</div>  
  
<script>  
    function checkPassword() {  
        const pass = document.getElementById('passcode').value;  
        // كلمة السر الافتراضية هي love، يمكنك تغييرها لاحقاً  
        if (pass.toLowerCase() === 'love') {  
            document.getElementById('lock-screen').classList.add('hidden');  
            document.getElementById('message-screen').classList.remove('hidden');  
        } else {  
            alert('كلمة السر خاطئة، حاول مرة أخرى!');  
        }  
    }  
</script>  
  
</body>  
</html>  
- [ ]   
