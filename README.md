<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Menu Tùy Chỉnh</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 20px;
            background-color: #f4f4f4;
        }
        .menu-container {
            border: 2px solid #4CAF50;
            border-radius: 10px;
            padding: 30px;
            background-color: white;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            display: none;
        }
        .menu {
            list-style-type: none;
            padding: 0;
        }
        .menu-item {
            margin: 20px 0;
            display: flex;
            justify-content: space-between;
            align-items: center;
            font-size: 18px;
        }
        .toggle {
            cursor: pointer;
            padding: 15px 20px;
            font-size: 16px;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
            transition: background-color 0.3s;
        }
        .toggle.off {
            background-color: #f44336;
        }
        .toggle:hover {
            opacity: 0.9;
        }
        .input-container {
            margin-bottom: 20px;
        }
    </style>
</head>
<body>

<h1 style="font-size: 24px;">Menu Tùy Chỉnh</h1>

<div class="input-container">
    <input type="text" id="keyInput" placeholder="Nhập khóa..." />
    <button onclick="checkKey()">Xác Nhận</button>
</div>

<div class="menu-container" id="menuContainer">
    <ul class="menu">
        <li class="menu-item">
            <span>Optimized Configuration</span>
            <button class="toggle" onclick="toggle(this)">Bật</button>
        </li>
        <li class="menu-item">
            <span>Setup DPI Config</span>
            <button class="toggle" onclick="toggle(this)">Bật</button>
        </li>
        <li class="menu-item">
            <span>Tối Ưu Hóa</span>
            <button class="toggle" onclick="toggle(this)">Bật</button>
        </li>
        <li class="menu-item">
            <span>Giảm Lố Đầu</span>
            <button class="toggle" onclick="toggle(this)">Bật</button>
        </li>
        <li class="menu-item">
            <span>Fix Rung Tâm</span>
            <button class="toggle" onclick="toggle(this)">Bật</button>
        </li>
    </ul>
</div>

<script>
    function checkKey() {
        const keyInput = document.getElementById('keyInput').value;
        const menuContainer = document.getElementById('menuContainer');
        if (keyInput === 'pda') {
            menuContainer.style.display = 'block';
        } else {
            alert('Khóa không đúng. Vui lòng thử lại.');
        }
    }

    function toggle(button) {
        button.classList.toggle('off');
        button.textContent = button.classList.contains('off') ? 'Tắt' : 'Bật';
    }
</script>

</body>
</html>
