<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bánh Pía Sóc Trăng - Tinh Hoa Ẩm Thực Quê Hương</title>
    <style>
        :root {
            --primary-color: #8b1515;
            --primary-dark: #5c0e0e;
            --accent-color: #d97724;
            --bg-color: #fcf9f5;
            --text-color: #333;
        }

* {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

  body {
            background-color: var(--bg-color);
            color: var(--text-color);
            line-height: 1.8;
            text-align: left;
        }

  /* PHẦN ĐẦU: TIÊU ĐỀ TRANG */
        header {
            background: linear-gradient(rgba(92, 14, 14, 0.9), rgba(139, 21, 21, 0.9)), url('anh-1.jpg') center/cover;
            color: #fff;
            padding: 40px 30px;
            text-align: left;
            box-shadow: 0 4px 10px rgba(0,0,0,0.15);
        }

  header h1 {
            font-size: 2.8rem;
            margin-bottom: 10px;
            letter-spacing: 1.5px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }

  header h2 {
            font-size: 1.4rem;
            font-weight: 400;
            margin-bottom: 8px;
            color: #fde8cd;
        }

  header p.sub-intro {
            font-size: 1.1rem;
            color: #f5f5f5;
            font-style: italic;
        }

  /* THANH ĐIỀU HƯỚNG NGANG */
        nav {
            background-color: var(--primary-dark);
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 5px rgba(0,0,0,0.2);
        }

  nav ul {
            list-style: none;
            display: flex;
            justify-content: flex-start;
            gap: 15px;
            flex-wrap: wrap;
            padding: 12px 30px;
        }

  nav ul li a {
            color: #fff;
            text-decoration: none;
            font-weight: 600;
            font-size: 0.95rem;
            padding: 6px 12px;
            border-radius: 4px;
            transition: all 0.3s ease;
        }

  nav ul li a:hover {
            background-color: var(--accent-color);
            color: #fff;
        }

  /* BỐ CỤC 3 CỘT: LỀ TRÁI (MENU) - NỘI DUNG CHÍNH - LỀ PHẢI (TÁC GIẢ & ĐĂNG NHẬP) */
        .wrapper {
            max-width: 1400px;
            margin: 30px auto;
            padding: 0 20px;
            display: grid;
            grid-template-columns: 240px 1fr 280px;
            gap: 25px;
        }

  /* LỀ TRÁI: MỤC LỤC / ĐIỀU HƯỚNG NHANH */
        .left-sidebar {
            background: #fff;
            padding: 20px;
            border-radius: 12px;
            box-shadow: 0 3px 10px rgba(0,0,0,0.05);
            border-top: 4px solid var(--accent-color);
            height: fit-content;
            position: sticky;
            top: 70px;
        }

  .left-sidebar h3 {
            font-size: 1.1rem;
            color: var(--primary-color);
            margin-bottom: 12px;
            padding-bottom: 6px;
            border-bottom: 2px solid #eee;
            text-align: left;
        }

  .left-sidebar ul {
            list-style: none;
        }

  .left-sidebar ul li {
            margin-bottom: 8px;
        }

  .left-sidebar ul li a {
            color: #555;
            text-decoration: none;
            font-size: 0.95rem;
            display: block;
            padding: 5px 8px;
            border-radius: 4px;
            transition: all 0.2s;
            text-align: left;
        }

  .left-sidebar ul li a:hover {
            background-color: #fcf2e8;
            color: var(--primary-color);
            padding-left: 12px;
        }

  /* NỘI DUNG CHÍNH (MAIN) */
        main {
            background: #fff;
            padding: 40px;
            border-radius: 12px;
            box-shadow: 0 3px 10px rgba(0,0,0,0.05);
            text-align: left;
        }

  .content-section {
            margin-bottom: 40px;
        }

  .content-section:last-child {
            margin-bottom: 0;
        }

  h2.section-heading {
            font-size: 1.6rem;
            color: var(--primary-color);
            border-left: 5px solid var(--accent-color);
            padding-left: 15px;
            margin-bottom: 20px;
            text-align: left;
        }

  p {
            margin-bottom: 15px;
            text-align: left;
            font-size: 1.05rem;
        }

  /* Khung chứa ảnh */
        .img-container {
            margin: 25px 0;
            text-align: left;
            background: #fdfbf7;
            padding: 15px;
            border: 1px solid #fae1cd;
            border-radius: 8px;
        }

  .img-container img {
            max-width: 100%;
            height: auto;
            max-height: 450px;
            border-radius: 6px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
            object-fit: cover;
            display: block;
        }

  .img-caption {
            margin-top: 10px;
            font-size: 0.95rem;
            color: #666;
            font-style: italic;
            text-align: left;
        }

  /* LỀ PHẢI (SIDEBAR): TÁC GIẢ & ĐĂNG NHẬP */
        aside {
            display: flex;
            flex-direction: column;
            gap: 25px;
            text-align: left;
        }

  .sidebar-card {
            background: #fff;
            padding: 20px;
            border-radius: 12px;
            box-shadow: 0 3px 10px rgba(0,0,0,0.05);
            border-top: 4px solid var(--primary-color);
        }

  .sidebar-title {
            font-size: 1.15rem;
            color: var(--primary-color);
            margin-bottom: 12px;
            padding-bottom: 6px;
            border-bottom: 2px solid #eee;
            text-align: left;
        }

  .author-list {
            list-style: none;
        }

  .author-list li {
            padding: 8px 0;
            border-bottom: 1px dashed #e5e5e5;
            font-size: 0.95rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

  .author-list li:last-child {
            border-bottom: none;
        }

  .leader-tag {
            background-color: var(--primary-color);
            color: white;
            font-size: 0.7rem;
            padding: 2px 6px;
            border-radius: 10px;
            font-weight: bold;
        }

  .login-form {
            display: flex;
            flex-direction: column;
            gap: 12px;
        }

  .login-form input {
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 6px;
            font-size: 0.95rem;
            outline: none;
            transition: border-color 0.3s;
        }

  .login-form input:focus {
            border-color: var(--primary-color);
        }

  .login-form button {
            background-color: var(--primary-color);
            color: white;
            border: none;
            padding: 10px;
            border-radius: 6px;
            font-weight: bold;
            font-size: 0.95rem;
            cursor: pointer;
            transition: background 0.3s;
        }

  .login-form button:hover {
            background-color: var(--primary-dark);
        }

  /* TÀI LIỆU THAM KHẢO */
        .references {
            background: #f4efe6;
            padding: 20px;
            border-radius: 8px;
            margin-top: 30px;
            font-size: 0.95rem;
            text-align: left;
        }

  .references ul {
            margin-left: 20px;
            margin-top: 10px;
        }

  .references li {
            margin-bottom: 8px;
            word-break: break-all;
        }

  .references a {
            color: var(--primary-color);
            text-decoration: none;
        }

  .references a:hover {
            text-decoration: underline;
        }

  /* PHẦN CHÂN TRANG */
        footer {
            background-color: #1a1a1a;
            color: #fff;
            text-align: left;
            padding: 25px 30px;
            margin-top: 40px;
            font-size: 1.1rem;
            font-weight: bold;
            letter-spacing: 1px;
            border-top: 4px solid var(--accent-color);
        }

  /* Responsive cho thiết bị nhỏ */
        @media (max-width: 1100px) {
            .wrapper {
                grid-template-columns: 1fr;
            }
            .left-sidebar {
                position: static;
            }
        }
    </style>
</head>
<body>
<!-- PHẦN ĐẦU: TIÊU ĐỀ VÀ GIỚI THIỆU -->
    <header id="trang-chu">
        <h1>BÁNH PÍA SÓC TRĂNG</h1>
        <h2>TINH HOA ẨM THỰC – HƯƠNG VỊ CỦA QUÊ HƯƠNG</h2>
        <p class="sub-intro">Một thức quà truyền thống mang dấu ấn văn hóa miền Tây Nam Bộ</p>
    </header>

   <nav>
        <ul>
            <li><a href="#trang-chu">Trang chủ</a></li>
            <li><a href="#mo-dau">Giới thiệu</a></li>
            <li><a href="#nguon-goc">1. Nguồn gốc</a></li>
            <li><a href="#huong-vi">2. Hương vị</a></li>
            <li><a href="#nguyen-lieu">3. Nguyên liệu</a></li>
            <li><a href="#quy-trinh">4. Quy trình</a></li>
            <li><a href="#tan-hue-vien">7. Tân Huê Viên</a></li>
        </ul>
    </nav>
<!-- BỐ CỤC 3 CỘT -->
    <div class="wrapper">
        <!-- LỀ TRÁI: THANH MỤC LỤC TRANG WEB -->
        <div class="left-sidebar">
            <h3>Danh Mục Nội Dung</h3>
            <ul>
                <li><a href="#mo-dau">Giới thiệu chung</a></li>
                <li><a href="#nguon-goc">1. Nguồn gốc</a></li>
                <li><a href="#huong-vi">2. Hương vị</a></li>
                <li><a href="#nguyen-lieu">3. Nguyên liệu</a></li>
                <li><a href="#quy-trinh">4. Quy trình làm bánh</a></li>
                <li><a href="#su-da-dang">5. Sự đa dạng</a></li>
                <li><a href="#doi-song">6. Văn hóa đời sống</a></li>
                <li><a href="#tan-hue-vien">7. Tân Huê Viên</a></li>
                <li><a href="#gia-tri-kinh-te">8. Giá trị kinh tế</a></li>
                <li><a href="#gin-giu">9. Gìn giữ tương lai</a></li>
            </ul>
        </div>
<!-- NỘI DUNG CHÍNH (MAIN) -->
        <main>
            <section class="content-section" id="mo-dau">
                <h2 class="section-heading">BÁNH PÍA SÓC TRĂNG – TINH HOA ẨM THỰC, HƯƠNG VỊ ĐẬM ĐÀ BẢN SẮC MIỀN TÂY</h2>
                <p>Nhắc đến Sóc Trăng, người ta không chỉ nhớ đến vùng đất miền Tây sông nước hiền hòa, nơi giao thoa của nhiều nền văn hóa, mà còn nhớ đến một thức quà đặc sản mang hương vị rất riêng – bánh pía. Với lớp vỏ mềm xốp, phần nhân thơm béo cùng vị ngọt bùi hòa quyện, bánh pía đã trở thành món quà quen thuộc, góp phần làm nên nét đặc sắc của ẩm thực địa phương[cite: 7].</p>
                <p>Không đơn thuần là một món bánh để thưởng thức, bánh pía còn chứa đựng câu chuyện về lịch sử, văn hóa và sự khéo léo của những người thợ làm bánh. Qua nhiều thế hệ, hương vị ấy vẫn được gìn giữ và lan tỏa, trở thành niềm tự hào của người dân Sóc Trăng[cite: 7].</p>

<div class="img-container">
                    <img src="anh-1.jpg" alt="Toàn cảnh bánh pía Sóc Trăng">
                    <div class="img-caption">Toàn cảnh bánh pía Sóc Trăng, đặc sản trứ danh miền Tây[cite: 7, 8]</div>
                </div>
            </section>

<section class="content-section" id="nguon-goc">
                <h2 class="section-heading">1. Nguồn gốc và hành trình phát triển</h2>
                <p>Bánh pía gắn liền với quá trình giao lưu văn hóa tại Nam Bộ. Theo các tư liệu giới thiệu về ẩm thực Sóc Trăng, món bánh theo chân cộng đồng người Hoa đến vùng đất phương Nam, rồi dần được điều chỉnh cách chế biến để phù hợp với khẩu vị và nguồn nguyên liệu địa phương. Qua thời gian, bánh pía trở thành một đặc sản tiêu biểu của Sóc Trăng[cite: 7].</p>
                <p>Từ những chiếc bánh được làm thủ công trong quy mô gia đình, nghề làm bánh pía dần phát triển thành hoạt động sản xuất chuyên nghiệp. Người thợ vẫn gìn giữ những kỹ thuật tạo vỏ và làm nhân đặc trưng, đồng thời cải tiến quy trình để đáp ứng nhu cầu ngày càng đa dạng[cite: 7].</p>

<div class="img-container">
                    <img src="anh-2.jpg" alt="Người thợ làm bánh truyền thống">
                    <div class="img-caption">Người thợ làm bánh theo phương pháp truyền thống[cite: 7, 9]</div>
                </div>
            </section>

<section class="content-section" id="huong-vi">
                <h2 class="section-heading">2. Hương vị đặc trưng làm nên sức hấp dẫn</h2>
                <p>Điều làm nên sức hấp dẫn của bánh pía chính là sự kết hợp hài hòa giữa lớp vỏ nhiều tầng và phần nhân mềm dẻo, thơm béo. Lớp vỏ được tạo nên từ những lớp bột mỏng, khi hoàn thiện có kết cấu mềm, tơi nhẹ và mang dáng vẻ đặc trưng[cite: 7].</p>
                <p>Phần nhân thường kết hợp đậu xanh nghiền nhuyễn với sầu riêng, tạo nên vị bùi ngọt và hương thơm nổi bật. Ở nhiều loại bánh, lòng đỏ trứng muối được đặt ở giữa nhân, đem lại vị mặn nhẹ và độ béo, giúp cân bằng vị ngọt[cite: 7].</p>

<div class="img-container">
                    <img src="anh-3.jpg" alt="Hương vị bánh pía">
                    <div class="img-caption">Hương vị thơm béo đặc trưng của bánh pía Sóc Trăng[cite: 7, 10]</div>
                </div>
            </section>

<section class="content-section" id="nguyen-lieu">
                <h2 class="section-heading">3. Những nguyên liệu quen thuộc</h2>
                <p>Mỗi chiếc bánh pía được tạo nên từ những nguyên liệu gần gũi nhưng cần được lựa chọn và phối hợp cẩn thận. Bột mì góp phần tạo nên lớp vỏ nhiều tầng; đậu xanh đem lại vị bùi và độ dẻo cho phần nhân; sầu riêng tạo hương thơm đặc trưng; còn trứng
