<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nhẹ Tâm Functions</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        function checkPassword() {
            const password = document.getElementById('password').value;
            if (password === 'DongAn') {
                document.getElementById('main-menu').classList.remove('hidden');
                document.getElementById('password-form').classList.add('hidden');
            } else {
                alert('Mật khẩu không đúng!');
            }
        }
    </script>
</head>
<body class="bg-gray-900 flex items-center justify-center min-h-screen">
    <div id="password-form" class="bg-black rounded-lg shadow-lg p-4 w-11/12 sm:w-1/4">
        <div class="bg-blue-700 text-white text-center py-2 rounded-t-lg text-lg">
            Nhập Mật Khẩu
        </div>
        <div class="p-2">
            <input type="password" id="password" class="w-full p-2 rounded mb-2 text-lg" placeholder="Mật khẩu">
            <button onclick="checkPassword()" class="w-full bg-blue-700 text-white py-2 rounded text-lg">Mở Khóa</button>
        </div>
    </div>
  <div id="main-menu" class="bg-black rounded-lg shadow-lg p-4 w-11/12 sm:w-1/4 hidden">
        <div class="bg-blue-700 text-white text-center py-2 rounded-t-lg text-lg">
            OPTIMIZED CONFIGURATION  @Pham_dong_an
        </div>
        <div class="p-2">
            <div class="flex items-center mb-2">
                <input type="checkbox" class="form-checkbox h-5 w-5 text-blue-600">
                <span class="ml-2 text-white text-lg">SETUP DPI CONFIG</span>
            </div>
            <div class="flex items-center mb-2">
                <input type="checkbox" class="form-checkbox h-5 w-5 text-blue-600">
                <span class="ml-2 text-white text-lg">TỐI ƯU HOÁ </span>
            </div>
            <div class="flex items-center mb-2">
                <input type="checkbox" class="form-checkbox h-5 w-5 text-blue-600">
                <span class="ml-2 text-white text-lg">GIẢM LỐ ĐẦU</span>
            </div>
            <div class="flex items-center mb-2">
                <input type="checkbox" class="form-checkbox h-5 w-5 text-blue-600">
                <span class="ml-2 text-white text-lg">NHẸ TÂM IOS</span>
            </div>
            <div class="flex items-center mb-2">
                <input type="checkbox" class="form-checkbox h-5 w-5 text-blue-600">
                <span class="ml-2 text-white text-lg">FIX RUNG TÂM</span>
            </div>
            <div class="text-red-600 text-center mt-2 text-lg">
                Zalo Admin: 0868.124.375
            </div>
        </div>
    </div>
</body>
</html>
