# marry-tasnim
READ ME
<!DOCTYPE html>
<html>
<head>
    <title>Will You Marry Me?</title>
    <style>
        body {
            margin: 0;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            background: linear-gradient(135deg, #ff9a9e, #fad0c4);
            font-family: Arial, sans-serif;
            overflow: hidden;
        }

        .container {
            text-align: center;
        }

        h1 {
            font-size: 2.5rem;
            color: white;
            margin-bottom: 40px;
        }

        .btn {
            padding: 15px 35px;
            font-size: 18px;
            border: none;
            border-radius: 30px;
            cursor: pointer;
            transition: 0.3s;
            position: absolute;
        }

        #yesBtn {
            background-color: #ff4d6d;
            color: white;
            left: 45%;
            top: 55%;
        }

        #noBtn {
            background-color: white;
            color: #ff4d6d;
            left: 55%;
            top: 55%;
        }

        .popup {
            display: none;
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background: white;
            padding: 40px;
            border-radius: 20px;
            box-shadow: 0 0 20px rgba(0,0,0,0.2);
            font-size: 20px;
            text-align: center;
        }

        .popup button {
            margin-top: 20px;
            padding: 10px 20px;
            border: none;
            background: #ff4d6d;
            color: white;
            border-radius: 20px;
            cursor: pointer;
        }
    </style>
</head>
<body>

<div class="container">
    <h1>Will you be my lifepartner Tasnim? 💍❤️</h1>
    <button class="btn" id="yesBtn">Yes ❤️</button>
    <button class="btn" id="noBtn">No 😏</button>
</div>

<div class="popup" id="popup">
    I knew it you will always choose me I love you ❤️
    <br>
    <button onclick="closePopup()">Close</button>
</div>

<script>
    const noBtn = document.getElementById("noBtn");
    const yesBtn = document.getElementById("yesBtn");
    const popup = document.getElementById("popup");

    noBtn.addEventListener("mouseover", function() {
        const x = Math.random() * (window.innerWidth - 100);
        const y = Math.random() * (window.innerHeight - 50);
        noBtn.style.left = x + "px";
        noBtn.style.top = y + "px";
    });

    yesBtn.addEventListener("click", function() {
        popup.style.display = "block";
    });

    function closePopup() {
        popup.style.display = "none";
    }
</script>

</body>
</html>
