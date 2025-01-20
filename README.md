
<html lang="vi">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Trang Web Của Tôi</title>
  <link href="https://fonts.googleapis.com/css2?family=Lora&display=swap" rel="stylesheet"> <!-- Thêm link font Lora -->
  <style>
    h1 {
      display: none;
    }
    body {
      font-family: 'Lora', serif; /* Sử dụng font Lora */
      margin: 0;
      padding: 0;
      background-image: url('Nền 4K.jpg'); /* Thêm hình ảnh nền */
      background-size: cover;
      background-position: center;
    }

    .container {
      display: flex;
      flex-direction: column;
      align-items: center;
      margin: 20px;
    }

    /* Pano đầu trang */
    .header {
      background-color: #2E3192; /* Màu nền pano */
      color: white;
      text-align: center;
      padding: 20px;
      position: relative;
      z-index: 2;
    }

    /* Chữ hiệu ứng bay lơ lửng */
    .floating-text {
      font-size: 36px;
      font-weight: bold;
      background-image: linear-gradient(45deg, red, orange, yellow, green, cyan, blue, violet);
      background-size: 200% 200%;
      color: transparent;
      background-clip: text;
      display: inline-block;
      animation: rainbow 3s linear infinite, float 2s ease-in-out infinite;
    }

    @keyframes rainbow {
      0% { background-position: 0% 50%; }
      100% { background-position: 100% 50%; }
    }

    @keyframes float {
      0% { transform: translateY(0); }
      50% { transform: translateY(-10px); }
      100% { transform: translateY(0); }
    }

    /* Dòng giới thiệu bản thân */
    .intro-container, .info-container {
      background-color: white; /* Màu nền trắng */
      padding: 20px;
      border-radius: 10px; /* Bo góc khung */
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); /* Đổ bóng */
      width: 100%;
      max-width: 800px;
      margin-bottom: 40px;
      border: 2px solid black; /* Viền màu đen */
    }

    .intro {
      font-size: 24px;
      color: black;
      text-align: center;
    }

    .section {
      display: flex;
      justify-content: center;
      align-items: center;
      width: 100%;
      margin-bottom: 40px;
      flex-wrap: wrap;
    }

    /* Nội dung chính */
    .first-section, .second-section {
      display: flex;
      justify-content: space-between;
      align-items: center;
      width: 100%;
    }

    .first-section .image, .second-section .image {
      flex: 1;
      text-align: center;
    }

    .first-section .text-container, .second-section .text-container {
      flex: 1;
      text-align: left;
    }

    .first-section .title, .second-section .title {
      font-size: 28px;
      font-weight: bold;
      color: red;
    }

    .first-section .text, .second-section .text {
      font-size: 20px;
      color: black;
    }

    /* Ảnh */
    .image img {
      width: 80%;
      height: auto;
      border-radius: 8px;
    }
  </style>
</head>
<body>

  <div class="header">
    <h1 class="floating-text">ĐẶNG HÙNG DINH XIN CHÀO</h1>
  </div>

  <div class="container">
    <!-- Giới thiệu bản thân -->
    <div class="intro-container">
      <div class="intro">
        Mình tên là Đặng Hùng Dinh, hiện đang theo học tại ngôi trường THPT Chuyên Bến Tre, mình rất hân hạnh được giới thiệu về bản thân mình.
      </div>
    </div>

    <!-- Thông tin cá nhân -->
    <div class="section first-section">
      <div class="image">
        <img src="c53a02299b14214a7805.jpg" alt="Ảnh 1">
      </div>
      <div class="text-container info-container">
        <div class="title">Thông tin cá nhân</div>
        <div class="text">
          Hiện tại mình học lớp 12 Lý, trường THPT Chuyên Bến Tre. Mình nặng 55kg và cao 1,70m. Mình là một Madridista đấy nhé và thần tượng của mình là Jude Bellingham.
        </div>
      </div>
    </div>

    <!-- Nguyện vọng tương lai -->
    <div class="section second-section">
      <div class="text-container info-container">
        <div class="title">Nguyện vọng tương lai</div>
        <div class="text">
          Mình chọn thi khối Khoa học tự nhiên, nguyện vọng 1 là ngành Sư phạm Đại học Sư Phạm và Đại học Luật.
        </div>
      </div>
      <div class="image">
        <img src="dinh.jpg" alt="Ảnh 2">
      </div>
    </div>

  </div>

</body>
</html>
