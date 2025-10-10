
<html lang="vi">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>wed hải anh coder</title>
  <style>
    #background-video {
  position: fixed;
  right: 0;
  bottom: 0;
  min-width: 100%;
  min-height: 100%;
  z-index: -1;
  object-fit: cover;
}

    body {
      margin: 0;
      padding: 0;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(90deg, #ff5f6d, #845ec2);
      color: #000;
      text-align: center;
    }

    h1 {
      padding: 20px;   
      font-style: italic;
    }

    .form-container {
      background: rgba(255, 255, 255, 0.1);
      width: 350px;
      margin: 30px auto;
      padding: 30px;
      border-radius: 20px;
      backdrop-filter: blur(10px);
      box-shadow: 0 4px 20px rgba(0,0,0,0.2);
      color: #000;
    }

    .form-container img {
      width: 80px;
      height: 80px;
      border-radius: 50%;
      margin-bottom: 10px;
    }

    .form-container input {
      width: 90%;
      margin: 10px 0;
      padding: 10px;
      border-radius: 10px;
      border: none;
      background: #ddd;
      font-size: 14px;
    }

    .form-container button {
      margin-top: 15px;
      padding: 10px 25px;
      background: #00e0ff;
      color: #fff;
      border: none;
      font-weight: bold;
      border-radius: 25px;
      cursor: pointer;
      font-size: 15px;
    }

    .form-container a {
      color: #000;
      text-decoration: underline;
      font-style: italic;
      cursor: pointer;
    }

    .contact {
      margin-top: 20px;
      font-size: 14px;
    }

    .contact i {
      margin-right: 5px;
    }

    #register-form {
      display: none;
    }

    .form-container p {
      margin-top: 15px;
    }
  </style>
</head>
<body>
    <!-- NỀN VIDEO -->
<video autoplay loop muted playsinline id="background-video">
  <source src="./cid-kagenou-the-eminence-in-shadow.960x540.mp4" type="video/mp4">
</video>


  <h1 style="color: white;">Chào mừng bạn đến với wed của hải anh coder</h1>

  <!-- Form Đăng Nhập -->
  <div class="form-container" id="login-form">
    <img src="./gojo-eyes-jujutsu-kaisen-4k-wallpaper-uhdpaper.com-208@2@a.jpg" alt="avatar">
    <h2>Đăng nhập</h2>
    <form action="tap2.html" target="_blank" method="post">
      <input type="text" placeholder="Tên đăng nhập" required>
      <input type="password" placeholder="Mật khẩu" required>
      <button>ĐĂNG NHẬP</button>
    </form>
    <p>Bạn chưa có tài khoản? <a onclick="toggleForm()">Đăng ký</a></p>
    <div class="contact">
      <p><i class="fa fa-phone"></i> 0986931896</p>
      <p><i class="fa fa-envelope"></i> haicube207@gamil.com</p>
      <p><em>Hãy sống hết mình vì coder</em></p>
    </div>
  </div>

  <!-- Form Đăng Ký --> 
  <div class="form-container" id="register-form">
    <img src="./gojo-eyes-jujutsu-kaisen-4k-wallpaper-uhdpaper.com-208@2@a.jpg" alt="avatar">
    <h2>Đăng ký tài khoản</h2>
    <form action="dangkithanhcong.html" target="_blank" method="get">
      <input type="text" placeholder="Họ và tên" required>
      <input type="text" placeholder="Tên đăng nhập" required>
    <input type="email" placeholder="Email" required>
    <input type="tel" placeholder="Số điện thoại" required>
    <input type="password" placeholder="Mật khẩu" required>
    <input type="password" placeholder="Xác nhận mật khẩu" required>
    <button>ĐĂNG KÝ</button>
    <p>Đã có tài khoản? <a onclick="toggleForm()">Đăng nhập</a></p>
  </div>

  <script>
    function toggleForm() {
      const loginForm = document.getElementById("login-form");
      const registerForm = document.getElementById("register-form");

      if (loginForm.style.display === "none") {
        loginForm.style.display = "block";
        registerForm.style.display = "none";
      } else {
        loginForm.style.display = "none";
        registerForm.style.display = "block";
      }
    }
  </script>
   <div class="wrap" role="main">
    <!-- Facebook icon (click opens Facebook profile) -->
    <a class="fb-icon" href="https://www.facebook.com/hai.ahhhh" target="_blank" rel="noopener noreferrer" title="Mở Facebook">
      <!-- simple 'f' svg -->
      <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M22 12.07C22 6.49 17.52 2 11.94 2S2 6.49 2 12.07c0 4.99 3.66 9.13 8.44 9.95v-7.04H8.1v-2.91h2.34V9.41c0-2.31 1.37-3.58 3.47-3.58.99 0 2.03.18 2.03.18v2.21h-1.13c-1.12 0-1.47.7-1.47 1.42v1.7h2.5l-.4 2.91h-2.1v7.04C18.34 21.2 22 17.07 22 12.07z"/></svg>
    </a>

    <div class="center-area" aria-live="polite">
      <!-- Laptop image card -->
      <div class="laptop-card" role="img" aria-label="Hình laptop hiển thị trang Facebook">
        <!-- Thay src bằng đường dẫn ảnh của bạn hoặc url -->
        <img src="./wallpapersden.com_satoru-gojo-jujutsu-kaisen-fortnite_1920x1080.jpg"
             alt="Laptop mở trang Facebook (ví dụ)">
      </div>

      <!-- Nút liên hệ: mở Facebook profile (mở tab mới) -->
      <a class="contact-btn" id="contactBtn" href="https://www.facebook.com/hai.ahhhh" target="_blank" rel="noopener noreferrer">
        liên hệ in4
      </a>
    </div>

    <!-- Nút chuyển trang nội bộ -> other.html -->
    <a class="goto" id="gotoBtn" href="tap3.html" title="Chuyển trang">
      trang share code →
    </a>
  </div>

  <script>
    // Thêm hành vi nếu bạn muốn: ví dụ logging / animation
    document.getElementById('contactBtn').addEventListener('click', function(e){
      // target mặc định mở tab mới vì attribute target="_blank"
      console.log('Người dùng nhấn "liên hệ in4" — mở liên kết Facebook.');
    });

    document.getElementById('gotoBtn').addEventListener('click', function(e){
      // mặc định link <a href="other.html"> sẽ chuyển trang
      console.log('Chuyển trang nội bộ sang other.html');
    });
  </script>

</body>
</html>
