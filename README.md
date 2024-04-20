- 👋 Hi, I’m @vaJatcripS
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
vaJatcripS/vaJatcripS is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>로그인 페이지</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            display: flex;
            align-items: center;
            justify-content: center;
            height: 100vh;
        }

        #login-container {
            background-color: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            width: 300px;
        }

        h2 {
            text-align: center;
            color: #333;
        }

        label {
            display: block;
            margin: 10px 0 5px;
            color: #666;
        }

        input {
            width: 100%;
            padding: 10px;
            margin-bottom: 10px;
            box-sizing: border-box;
        }

        button {
            width: 100%;
            padding: 10px;
            background-color: #4caf50;
            color: #fff;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        button:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <div id="login-container">
        <h2>로그인</h2>
        <form>
            <label for="username">사용자 이름:</label>
            <input type="text" id="username" name="username" required>
            <label for="password">비밀번호:</label>
            <input type="password" id="password" name="password" required>
            <button type="button" id="submit-btn">로그인</button>
        </form>
    </div>
    <script>
        /** function when click #submit-btn */
        document.getElementById('submit-btn').addEventListener('click', function login() {
            var username = document.getElementById('username').value;
            var password = document.getElementById('password').value;

            if (username === 'user' && password === 'password') {
                alert('로그인 완료');
            } else {
                alert('로그인 실패.');
            }
        })
    </script>
</body>
</html>
