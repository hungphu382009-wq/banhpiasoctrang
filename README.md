<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bánh Pía - Đặc Sản Sóc Trăng</title>
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: #f9f6f0;
            color: #333;
            line-height: 1.6;
        }

        /* PHẦN ĐẦU (HEADER & NAVIGATION) */
        header {
            background-color: #8b1515;
            color: #fff;
            padding: 25px 20px 15px 20px;
            text-align: center;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }

        header h1 {
            font-size: 2.2rem;
            margin-bottom: 8px;
            letter-spacing: 1px;
        }

        header p.intro {
            font-size: 1.05rem;
            max-width: 800px;
            margin: 0 auto 15px auto;
            color: #fde8cd;
        }

        nav {
            background-color: #5c0e0e;
            padding: 10px 0;
            position: sticky;
            top: 0;
            z-index: 100;
        }

        nav ul {
            list-style: none;
            display: flex;
            justify-content: center;
            gap: 25px;
            flex-wrap: wrap;
        }

        nav ul li a {
            color: #fff;
            text-decoration: none;
            font-weight: bold;
            font-size: 1rem;
            padding: 6px 12px;
            border-radius: 4px;
            transition: background-color 0.3s;
        }

        nav ul li a:hover {
            background-color: #d97724;
        }

        /* CONTAINER CHÍNH */
        .container {
            max-width: 1100px;
            margin: 25px auto;
            padding: 0 20px;
            display: grid;
            grid-template-columns: 2fr 1fr;
            gap: 25px;
        }

        /* PHẦN THÂN (CONTENT) */
        main {
            background: #fff;
            padding: 25px;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.05);
        }

        .section-title {
            font-size: 1.5rem;
            color: #8b1515;
            border-bottom: 2px solid #8b1515;
            padding-bottom: 5px;
            margin-bottom: 15px;
            margin-top: 20px;
        }

        .section-title:first-child {
            margin-top: 0;
        }

        .post-content p {
            margin-bottom: 15px;
            text-align: justify;
        }

        .post-content ul {
            margin-left: 20px;
            margin-bottom: 15px;
        }

        .post-content li {
            margin-bottom: 6px;
        }

        /* KHU VỰC HÌNH ẢNH BÁNH PÍA */
        .image-gallery {
            display: grid;
            grid-template-columns: 1fr;
            gap: 20px;
            margin: 20px 0;
        }

        .image-card {
            background-color: #fff8f0;
            border: 1px solid #ffe3c6;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 3px 6px rgba(0,0,0,0.08);
        }

        .image-card img {
            width: 100%;
            height: 280px;
            object-fit: cover;
            display: block;
        }

        .image-card .caption {
            padding: 10px 15px;
            font-size: 0.95rem;
            color: #555;
            text-align: center;
            font-style: italic;
        }

        /* CỘT BÊN (SIDEBAR) */
        aside {
            display: flex;
            flex-direction: column;
            gap: 20px;
        }

        .card {
            background: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.05);
        }

        .authors-list {
            list-style: none;
        }

        .authors-list li {
            padding: 8px 0;
            border-bottom: 1px dashed #eee;
            font-size: 0.95rem;
        }

        .authors-list li:last-child {
            border-bottom: none;
        }

        .leader-badge {
            background-color: #8b1515;
            color: white;
            font-size: 0.75rem;
            padding: 2px 6px;
            border-radius: 3px;
            margin-left: 5px;
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
            border-radius: 4px;
            font-size: 0.95rem;
        }

        .login-form button {
            background-color: #8b1515;
            color: white;
            border: none;
            padding: 10px;
            border-radius: 4px;
            font-weight: bold;
            cursor: pointer;
            transition: background 0.3s;
        }

        .login-form button:hover {
            background-color: #a82020;
        }

        /* CHÂN TRANG */
        footer {
            background-color: #222;
            color: #fff;
            text-align: center;
            padding: 20px;
            margin-top: 30px;
            font-size: 1.1rem;
            font-weight: bold;
            letter-spacing: 1px;
        }

        @media (max-width: 768px) {
            .container {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>

    <!-- PHẦN ĐẦU (Header & Thanh điều hướng) -->
    <header id="trang-chu">
        <h1>BÁNH PÍA SÓC TRĂNG</h1>
        <p class="intro">Bánh Pía là thức quà đặc sản nổi tiếng của vùng đất Sóc Trăng, mang nét văn hóa ẩm thực độc đáo kết hợp giữa người Hoa và người Nam Bộ.</p>
    </header>

    <nav>
        <ul>
            <li><a href="#trang-chu">Trang chủ</a></li>
            <li><a href="#gioi-thieu">Giới thiệu</a></li>
            <li><a href="#hinh-anh">Hình ảnh</a></li>
            <li><a href="#tac-gia">Tác giả</a></li>
            <li><a href="#dang-nhap">Đăng nhập</a></li>
        </ul>
    </nav>

    <!-- PHẦN THÂN -->
    <div class="container">
        
        <main>
            <!-- NỘI DUNG GIỚI THIỆU -->
            <section id="gioi-thieu" class="post-content">
                <h2 class="section-title">Nguồn Gốc & Ý Nghĩa</h2>
                <p>Từ "Pía" có nguồn gốc từ tiếng Triều Châu "Pi-é", nghĩa là bánh mỳ tròn hay bánh nướng. Bánh do người Triều Châu mang theo khi di cư đến vùng sông nước Sóc Trăng vào thế kỷ 17. Qua thời gian, người dân địa phương đã sáng tạo thêm nhân sầu riêng, đậu xanh và trứng muối để tạo nên hương vị đặc trưng như ngày nay.</p>

                <h2 class="section-title">Đặc Điểm Của Bánh Pía</h2>
                <ul>
                    <li><strong>Vỏ bánh:</strong> Độc đáo với hàng chục lớp vỏ mỏng xếp chồng lên nhau như từng trang sách, mềm dẻo và không bị khô.</li>
                    <li><strong>Nhân bánh:</strong> Được nhào nặn từ đậu xanh hấp chín xay mịn, mỡ lợn xắt hạt lựu, hòa quyện cùng cơm sầu riêng tươi đậm đà.</li>
                    <li><strong>Lòng đỏ trứng muối:</strong> Nằm ở chính giữa chiếc bánh, mang vị mặn bùi giúp cân bằng độ ngọt béo của sầu riêng và đậu xanh.</li>
                </ul>

                <h2 class="section-title">Thưởng Thức Bánh Pía Đúng Cách</h2>
                <p>Bánh Pía ngon nhất là khi thưởng thức cùng một tách trà nóng (như trà xanh hoặc trà ổi). Vị chát nhẹ, ấm áp của trà sẽ làm dịu đi độ ngọt và béo ngậy của bánh, tôn lên hương thơm sầu riêng đọng lại nơi đầu lưỡi.</p>
            </section>

            <!-- HÌNH ẢNH BÁNH PÍA CHUẨN -->
            <section id="hinh-anh">
                <h2 class="section-title">Hình Ảnh Bánh Pía Chuẩn</h2>
                <div class="image-gallery">
                    <div class="image-card">
                        <img src="https://images.unsplash.com/photo-1509440159596-0249088772ff?auto=format&fit=crop&w=1000&q=80" alt="Bánh Pía nướng vàng óng">
                        <div class="caption">Hình 1: Chiếc Bánh Pía tròn đầy với vỏ nướng màu vàng cam đẹp mắt</div>
                    </div>
                    
                    <div class="image-card">
                        <img src="https://images.unsplash.com/photo-1621236378699-8597faf6a176?auto=format&fit=crop&w=1000&q=80" alt="Chi tiết nhân bánh pía sầu riêng trứng muối">
                        <div class="caption">Hình 2: Cắt đôi chiếc bánh thấy rõ lớp vỏ ngàn lớp cùng nhân trứng muối bùi béo bên trong</div>
                    </div>
                </div>
            </section>
        </main>

        <!-- CỘT BÊN (TÁC GIẢ & ĐĂNG NHẬP) -->
        <aside>
            <!-- Phần Tác giả -->
            <div class="card" id="tac-gia">
                <h3 class="section-title" style="font-size: 1.2rem; margin-top: 0;">Tác Giả Thực Hiện</h3>
                <ul class="authors-list">
                    <li><strong>Hưng Phú</strong> <span class="leader-badge">Trưởng nhóm</span></li>
                    <li>Thảo Vy</li>
                    <li>Ngọc Hương</li>
                    <li>Lý Thư</li>
                    <li>Gia Bảo</li>
                    <li>Hân Bùi</li>
                    <li>Xuân Mai</li>
                </ul>
            </div>

            <!-- Phần Đăng nhập -->
            <div class="card" id="dang-nhap">
                <h3 class="section-title" style="font-size: 1.2rem; margin-top: 0;">Đăng Nhập</h3>
                <form class="login-form" action="#" method="post" onsubmit="return false;">
                    <input type="text" placeholder="Tên đăng nhập" required>
                    <input type="password" placeholder="Mật khẩu" required>
                    <button type="submit">Đăng Nhập</button>
                </form>
            </div>
        </aside>

    </div>

    <!-- PHẦN CHÂN TRANG -->
    <footer>
        DS -> Lớp 12A2 -> THPT HOANG DIEU
    </footer>

</body>
</html>
