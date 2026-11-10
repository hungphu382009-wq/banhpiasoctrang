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
            text-align: left; /* Căn lề trái toàn bộ trang web */
        }

  /* PHẦN ĐẦU (HEADER) */
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

  /* THANH ĐIỀU HƯỚNG NGANG (NAV) */
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

  /* BỐ CỤC 3 CỘT: MỤC LỤC LỀ TRÁI - NỘI DUNG CHÍNH - LỀ PHẢI (TÁC GIẢ & ĐĂNG NHẬP) */
        .wrapper {
            max-width: 1400px;
            margin: 30px auto;
            padding: 0 20px;
            display: grid;
            grid-template-columns: 240px 1fr 280px;
            gap: 25px;
        }

  /* THANH MỤC LỤC TRÊN LỀ TRÁI */
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
            font-size: 0.92rem;
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

  /* PHẦN THÂN NỘI DUNG CHÍNH (MAIN) */
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

  /* KHUNG CHỨA HÌNH ẢNH */
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

  /* CỘT BÊN PHẢI (SIDEBAR): TÁC GIẢ & ĐĂNG NHẬP */
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

  /* PHẦN CHÂN TRANG (FOOTER) */
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
 <!-- PHẦN ĐẦU (HEADER) -->
    <header id="trang-chu">
        <h1>BÁNH PÍA SÓC TRĂNG</h1>
        <h2>TINH HOA ẨM THỰC – HƯƠNG VỊ CỦA QUÊ HƯƠNG</h2>
        <p class="sub-intro">Một thức quà truyền thống mang dấu ấn văn hóa miền Tây Nam Bộ</p>
    </header>
<!-- THANH ĐIỀU HƯỚNG -->
    <nav>
        <ul>
            <li><a href="#trang-chu">Trang chủ</a></li>
            <li><a href="#mo-dau">Giới thiệu</a></li>
            <li><a href="#nguon-goc">1. Nguồn gốc</a></li>
            <li><a href="#huong-vi">2. Hương vị</a></li>
            <li><a href="#nguyen-lieu">3. Nguyên liệu</a></li>
            <li><a href="#quy-trinh">4. Quy trình</a></li>
            <li><a href="#su-da-dang">5. Đa dạng</a></li>
            <li><a href="#doi-song">6. Văn hóa</a></li>
            <li><a href="#tan-hue-vien">7. Tân Huê Viên</a></li>
            <li><a href="#gia-tri-kinh-te">8. Kinh tế</a></li>
            <li><a href="#gin-giu">9. Tương lai</a></li>
        </ul>
    </nav>
<!-- BỐ CỤC 3 CỘT -->
    <div class="wrapper">
        <!-- CỘT BÊN TRÁI: MỤC LỤC TRANG WEB -->
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
                <li><a href="#loi-ket">Lời kết</a></li>
            </ul>
        </div>
<!-- PHẦN THÂN NỘI DUNG CHÍNH (MAIN) -->
        <main>
            <!-- Giới thiệu đầu bài -->
            <section class="content-section" id="mo-dau">
                <h2 class="section-heading">BÁNH PÍA SÓC TRĂNG – TINH HOA ẨM THỰC, HƯƠNG VỊ ĐẬM ĐÀ BẢN SẮC MIỀN TÂY</h2>
                <p>Nhắc đến Sóc Trăng, người ta không chỉ nhớ đến vùng đất miền Tây sông nước hiền hòa, nơi giao thoa của nhiều nền văn hóa, mà còn nhớ đến một thức quà đặc sản mang hương vị rất riêng – bánh pía. Với lớp vỏ mềm xốp, phần nhân thơm béo cùng vị ngọt bùi hòa quyện, bánh pía đã trở thành món quà quen thuộc, góp phần làm nên nét đặc sắc của ẩm thực địa phương[cite: 7].</p>
                <p>Không đơn thuần là một món bánh để thưởng thức, bánh pía còn chứa đựng câu chuyện về lịch sử, văn hóa và sự khéo léo của những người thợ làm bánh. Qua nhiều thế hệ, hương vị ấy vẫn được gìn giữ và lan tỏa, trở thành niềm tự hào của người dân Sóc Trăng[cite: 7].</p>
<!-- Ảnh 1 -->
                <div class="img-container">
                    <img src="anh-1.jpg" alt="Toàn cảnh bánh pía Sóc Trăng">
                    <div class="img-caption">Toàn cảnh bánh pía Sóc Trăng, đặc sản trứ danh miền Tây[cite: 7, 8]</div>
                </div>
            </section>
<!-- 1. Nguồn gốc và hành trình phát triển -->
            <section class="content-section" id="nguon-goc">
                <h2 class="section-heading">1. Nguồn gốc và hành trình phát triển</h2>
                <p>Bánh pía gắn liền với quá trình giao lưu văn hóa tại Nam Bộ. Theo các tư liệu giới thiệu về ẩm thực Sóc Trăng, món bánh theo chân cộng đồng người Hoa đến vùng đất phương Nam, rồi dần được điều chỉnh cách chế biến để phù hợp với khẩu vị và nguồn nguyên liệu địa phương. Qua thời gian, bánh pía trở thành một đặc sản tiêu biểu của Sóc Trăng[cite: 7].</p>
                <p>Từ những chiếc bánh được làm thủ công trong quy mô gia đình, nghề làm bánh pía dần phát triển thành hoạt động sản xuất chuyên nghiệp. Người thợ vẫn gìn giữ những kỹ thuật tạo vỏ và làm nhân đặc trưng, đồng thời cải tiến quy trình để đáp ứng nhu cầu ngày càng đa dạng. Hành trình ấy cho thấy sức sống bền bỉ của một món ăn truyền thống khi được cộng đồng trân trọng và tiếp nối[cite: 7].</p>
<!-- Ảnh 2 -->
                <div class="img-container">
                    <img src="anh-2.jpg" alt="Người thợ làm bánh truyền thống">
                    <div class="img-caption">Người thợ làm bánh theo phương pháp truyền thống[cite: 7, 9]</div>
                </div>
            </section>
<!-- 2. Hương vị đặc trưng làm nên sức hấp dẫn -->
            <section class="content-section" id="huong-vi">
                <h2 class="section-heading">2. Hương vị đặc trưng làm nên sức hấp dẫn</h2>
                <p>Điều làm nên sức hấp dẫn của bánh pía chính là sự kết hợp hài hòa giữa lớp vỏ nhiều tầng và phần nhân mềm dẻo, thơm béo. Lớp vỏ được tạo nên từ những lớp bột mỏng, khi hoàn thiện có kết cấu mềm, tơi nhẹ và mang dáng vẻ đặc trưng[cite: 7].</p>
                <p>Phần nhân thường kết hợp đậu xanh nghiền nhuyễn với sầu riêng, tạo nên vị bùi ngọt và hương thơm nổi bật. Ở nhiều loại bánh, lòng đỏ trứng muối được đặt ở giữa nhân, đem lại vị mặn nhẹ và độ béo, giúp cân bằng vị ngọt. Tùy công thức, người làm bánh còn kết hợp khoai môn hoặc những nguyên liệu khác để tạo thêm lựa chọn cho thực khách[cite: 7].</p>
                <p>Khi thưởng thức, người ăn có thể cảm nhận vị mềm của vỏ bánh, vị bùi của đậu xanh, hương thơm đặc trưng của sầu riêng và chút mặn béo từ trứng muối. Sự hòa quyện ấy tạo nên dấu ấn riêng khó nhầm lẫn[cite: 7].</p>
<!-- Ảnh 3 -->
                <div class="img-container">
                    <img src="anh-3.jpg" alt="Hương vị bánh pía">
                    <div class="img-caption">Hương vị thơm béo đặc trưng của bánh pía Sóc Trăng[cite: 7, 10]</div>
                </div>
            </section>
<!-- 3. Những nguyên liệu quen thuộc -->
            <section class="content-section" id="nguyen-lieu">
                <h2 class="section-heading">3. Những nguyên liệu quen thuộc</h2>
                <p>Mỗi chiếc bánh pía được tạo nên từ những nguyên liệu gần gũi nhưng cần được lựa chọn và phối hợp cẩn thận. Bột mì góp phần tạo nên lớp vỏ nhiều tầng; đậu xanh đem lại vị bùi và độ dẻo cho phần nhân; sầu riêng tạo hương thơm đặc trưng; còn trứng muối bổ sung vị mặn nhẹ, làm phong phú tổng thể hương vị. Khoai môn và một số nguyên liệu khác cũng được sử dụng để tạo nên những dòng bánh đa dạng[cite: 7].</p>
                <p>Chất lượng nguyên liệu, tỷ lệ phối trộn và kinh nghiệm của người thợ đều ảnh hưởng đến hương vị cuối cùng. Bởi vậy, sự hấp dẫn của bánh pía không chỉ đến từ từng thành phần riêng lẻ mà còn từ cách chúng hòa quyện với nhau[cite: 7].</p>
<!-- Ảnh 4 -->
                <div class="img-container">
                    <img src="anh-4.jpg" alt="Nguyên liệu làm bánh pía">
                    <div class="img-caption">Bột mì, đậu xanh, sầu riêng, trứng muối và khoai môn được bày riêng[cite: 7, 11]</div>
                </div>
            </section>
<!-- 4. Quy trình làm bánh – sự tỉ mỉ trong từng công đoạn -->
            <section class="content-section" id="quy-trinh">
                <h2 class="section-heading">4. Quy trình làm bánh – sự tỉ mỉ trong từng công đoạn</h2>
                <p>Đằng sau mỗi chiếc bánh pía hoàn chỉnh là một quá trình chế biến đòi hỏi sự cẩn thận và kinh nghiệm. Trước tiên, nguyên liệu được lựa chọn và sơ chế. Đậu xanh được nấu chín, nghiền mịn rồi phối trộn với các thành phần khác để tạo thành phần nhân dẻo thơm[cite: 7].</p>
                <p>Tiếp theo, người thợ chuẩn bị phần vỏ và kết hợp các lớp bột theo kỹ thuật phù hợp để tạo kết cấu nhiều tầng. Nhân bánh được đặt vào giữa, sau đó bánh được bọc kín và tạo hình. Công đoạn nướng cần được kiểm soát phù hợp để bánh chín đều, có màu sắc đẹp và giữ được kết cấu đặc trưng[cite: 7].</p>
                <p>Mỗi công đoạn đều thể hiện sự kiên nhẫn, khéo léo và kinh nghiệm của người làm bánh. Ngày nay, bên cạnh kỹ thuật thủ công, nhiều cơ sở còn ứng dụng máy móc và quy trình sản xuất hiện đại nhằm nâng cao năng suất, tính đồng đều và chất lượng sản phẩm[cite: 7].</p>
<!-- Ảnh 5 -->
                <div class="img-container">
                    <img src="anh-5.jpg" alt="Quy trình làm bánh pía">
                    <div class="img-caption">Các bước chuẩn bị nhân, cán bột, bọc bánh, tạo hình và nướng bánh[cite: 7, 12]</div>
                </div>
            </section>
<!-- 5. Sự đa dạng trong thế giới bánh pía -->
            <section class="content-section" id="su-da-dang">
                <h2 class="section-heading">5. Sự đa dạng trong thế giới bánh pía</h2>
                <p>Cùng với sự phát triển của thị trường, bánh pía ngày nay có nhiều hương vị để đáp ứng sở thích của người thưởng thức. Bánh pía sầu riêng nổi bật với hương thơm nồng nàn và vị béo; bánh pía khoai môn có vị bùi dịu; bánh pía đậu xanh mang hương vị gần gũi, ngọt thanh; trong khi bánh pía trứng muối tạo điểm nhấn nhờ sự kết hợp giữa vị ngọt của nhân và vị mặn béo của trứng[cite: 7].</p>
                <p>Dù có nhiều biến tấu, các loại bánh pía vẫn giữ nét đặc trưng ở lớp vỏ nhiều tầng và phần nhân mềm dẻo. Sự phong phú ấy giúp món bánh truyền thống tiếp tục gần gũi với nhiều thế hệ thực khách[cite: 7].</p>
<!-- Ảnh 6 -->
                <div class="img-container">
                    <img src="anh-6.jpg" alt="Sự đa dạng của bánh pía">
                    <div class="img-caption">Các dòng bánh pía đa dạng chuẩn bị cho người thưởng thức[cite: 7, 15]</div>
                </div>
            </section>
<!-- 6. Bánh pía trong đời sống và văn hóa -->
            <section class="content-section" id="doi-song">
                <h2 class="section-heading">6. Bánh pía trong đời sống và văn hóa</h2>
                <p>Bánh pía không chỉ là một món ăn mà còn hiện diện trong những khoảnh khắc đời thường của người dân miền Tây. Những hộp bánh được mang về sau chuyến đi, đặt trên bàn trà khi gia đình sum họp hay trao tặng người thân, bạn bè đã trở thành hình ảnh quen thuộc[cite: 7].</p>
                <p>Đối với nhiều người, hương vị bánh pía gợi nhớ quê nhà, những buổi trò chuyện bên tách trà và sự chân tình trong cách người miền Tây đón tiếp khách. Món bánh cũng là một dấu ấn của quá trình giao lưu văn hóa tại Sóc Trăng, nơi nhiều cộng đồng cùng sinh sống, đóng góp vào sự phong phú của đời sống ẩm thực địa phương[cite: 7].</p>
<!-- Ảnh 7 -->
                <div class="img-container">
                    <img src="anh-7.jpg" alt="Bánh pía trong văn hóa">
                    <div class="img-caption">Bánh pía dùng cùng trà hoặc hộp bánh được trao tặng trong dịp thăm hỏi[cite: 7, 13]</div>
                </div>
            </section>
<!-- 7. Tân Huê Viên – thương hiệu gắn với đặc sản Sóc Trăng -->
            <section class="content-section" id="tan-hue-vien">
                <h2 class="section-heading">7. Tân Huê Viên – thương hiệu gắn với đặc sản Sóc Trăng</h2>
                <p>Nhắc đến bánh pía Sóc Trăng, Tân Huê Viên là một trong những thương hiệu được nhiều người biết đến. Cơ sở sản xuất bánh pía Tân Huê Viên được thành lập năm 1985, khởi đầu từ quy mô nhỏ và từng bước phát triển thành doanh nghiệp chuyên chế biến thực phẩm. Hành trình ấy gắn với sự kiên trì, nỗ lực duy trì chất lượng và mong muốn đưa đặc sản địa phương đến với đông đảo người tiêu dùng[cite: 7].</p>
                <p>Bên cạnh bánh pía, Tân Huê Viên còn phát triển nhiều sản phẩm khác như lạp xưởng, bánh in, bánh trung thu và các loại bánh kẹo đặc sản. Doanh nghiệp từng bước đầu tư trang thiết bị, cải tiến quy trình sản xuất và mở rộng thị trường trong nước cũng như quốc tế[cite: 7].</p>
                <p>Tân Huê Viên là một ví dụ cho thấy một nghề truyền thống có thể phát triển theo hướng hiện đại mà vẫn giữ được dấu ấn ẩm thực quê hương. Sự phát triển của thương hiệu cũng góp phần quảng bá hình ảnh bánh pía và đặc sản Sóc Trăng đến nhiều thực khách[cite: 7].</p>
                <p>Một dấu mốc đáng chú ý là vào tháng 1 năm 2026, nhân dịp kỷ niệm 40 năm hình thành thương hiệu, Tân Huê Viên thực hiện chiếc bánh pía có trọng lượng 368 kg, được giới thiệu là phá kỷ kỷ kỷ kỷ lục bánh pía lớn nhất Việt Nam trước đó. Sự kiện thể hiện tinh thần sáng tạo và nỗ lực tôn vinh nghề bánh truyền thống[cite: 7].</p>
<!-- Ảnh 8 -->
                <div class="img-container">
                    <img src="anh-8.jpg" alt="Khuôn viên Tân Huê Viên">
                    <div class="img-caption">Cổng hoặc khuôn viên Tân Huê Viên; ưu tiên ảnh chụp thực tế[cite: 7, 14]</div>
                </div>
            </section>
<!-- 8. Giá trị kinh tế và vị thế của bánh pía Sóc Trăng -->
            <section class="content-section" id="gia-tri-kinh-te">
                <h2 class="section-heading">8. Giá trị kinh tế và vị thế của bánh pía Sóc Trăng</h2>
                <p>Sự nổi tiếng của bánh pía góp phần thúc đẩy hoạt động sản xuất, kinh doanh và quảng bá đặc sản địa phương. Các cơ sở làm bánh tạo thêm việc làm, duy trì kỹ năng nghề truyền thống và đưa sản phẩm đến nhiều tỉnh thành. Bánh pía cũng thường được du khách lựa chọn làm quà khi ghé thăm Sóc Trăng[cite: 7].</p>
                <p>Không chỉ mang lại giá trị kinh tế, bánh pía còn góp phần giới thiệu hình ảnh vùng đất và con người Sóc Trăng. Mỗi chiếc bánh được trao đi là một dịp để câu chuyện về món ăn, nghề làm bánh và nét văn hóa địa phương được lan tỏa[cite: 7].</p>
<!-- Ảnh 9 -->
                <div class="img-container">
                    <img src="anh-9.jpg" alt="Giá trị kinh tế bánh pía">
                    <div class="img-caption">Cơ sở sản xuất, khu đóng gói hoặc quầy trưng bày bánh pía[cite: 7]</div>
                </div>
            </section>
<!-- 9. Gìn giữ hương vị truyền thống, hướng đến tương lai -->
            <section class="content-section" id="gin-giu">
                <h2 class="section-heading">9. Gìn giữ hương vị truyền thống, hướng đến tương lai</h2>
                <p>Trong bối cảnh thị trường ngày càng phát triển, người tiêu dùng quan tâm nhiều hơn đến chất lượng nguyên liệu, quy trình sản xuất, bao bì và an toàn thực phẩm. Vì vậy, các cơ sở sản xuất cần không ngừng nâng cao chất lượng, cải tiến công nghệ và xây dựng thương hiệu[cite: 7].</p>
                <p>Tuy nhiên, đổi mới không có nghĩa là đánh mất bản sắc. Hương vị truyền thống, kinh nghiệm của người thợ và những kỹ thuật làm bánh đặc trưng vẫn cần được trân trọng, gìn giữ và truyền lại cho thế hệ sau. Việc giới thiệu bánh pía trên các nền tảng số cũng là một cách để người trẻ tìm hiểu, quảng bá và góp phần bảo tồn đặc sản quê hương[cite: 7].</p>
<!-- Ảnh 10 -->
                <div class="img-container">
                    <img src="anh-10.jpg" alt="Gìn giữ nghề truyền thống">
                    <div class="img-caption">Người thợ làm bánh thủ công kết hợp với hình ảnh dây chuyền sản xuất hiện đại[cite: 7]</div>
                </div>
            </section>
<!-- Lời kết -->
            <section class="content-section" id="loi-ket">
                <h2 class="section-heading">Lời kết – Bánh pía, hương vị quê hương còn mãi</h2>
                <p>Có những món ăn khiến người ta nhớ đến bởi hương vị, nhưng cũng có những món ăn lưu giữ trong lòng người thưởng thức cả một miền ký ức. Bánh pía Sóc Trăng chính là một thức quà như thế. Từ lớp vỏ mềm xốp, phần nhân thơm béo đến vị ngọt bùi hòa quyện, tất cả tạo nên nét đặc trưng đã gắn bó với vùng đất này qua nhiều thế hệ[cite: 7].</p>
                <p>Mỗi chiếc bánh là kết tinh của nguyên liệu, kỹ thuật, sự khéo léo và tình yêu dành cho nghề truyền thống. Dù thời gian đổi thay, bánh pía vẫn tiếp tục hiện diện trong đời sống, trong những dịp sum họp và trong hành trang của những người con xa quê[cite: 7].</p>
                <p style="font-weight: bold; color: var(--primary-color); text-align: left; font-size: 1.15rem; margin-top: 15px;">
                    BÁNH PÍA SÓC TRĂNG – GÓI TRỌN HƯƠNG VỊ QUÊ HƯƠNG TRONG TỪNG CHIẾC BÁNH.
                </p>
<!-- Ảnh 11 -->
                <div class="img-container">
                    <img src="anh-11.jpg" alt="Lời kết bánh pía Sóc Trăng">
                    <div class="img-caption">BÁNH PÍA SÓC TRĂNG – GÓI TRỌN HƯƠNG VỊ QUÊ HƯƠNG TRONG TỪNG CHIẾC BÁNH[cite: 7].</div>
                </div>
            </section>
<!-- Tư liệu tham khảo -->
            <div class="references">
                <strong>TƯ LIỆU THAM KHẢO</strong>
                <p style="margin-top: 5px; font-size: 0.9rem;">Các thông tin về nguồn gốc bánh pía và thương hiệu Tân Huê Viên được đối chiếu từ những tư liệu giới thiệu về ẩm thực Sóc Trăng và lịch sử doanh nghiệp[cite: 7]:</p>
                <ul>
                    <li>Bánh pía Sóc Trăng – Vietnam Pictorial (Thông tấn xã Việt Nam): <a href="https://vietnam.vnanet.vn/vietnamese/tin-tuc/banh-pia-soc-trang-33987.html" target="_blank">https://vietnam.vnanet.vn/vietnamese/tin-tuc/banh-pia-soc-trang-33987.html</a>[cite: 7]</li>
                    <li>Giới thiệu bánh Pía Tân Huê Viên – website Tân Huê Viên: <a href="https://www.banhpia.vn/gioi-thieu-banh-pia-tan-hue-vien/" target="_blank">https://www.banhpia.vn/gioi-thieu-banh-pia-tan-hue-vien/</a>[cite: 7]</li>
                    <li>Tân Huê Viên: 37 năm đưa thương hiệu đặc sản bánh pía Sóc Trăng vươn tầm: <a href="https://vienkyluc.vn/tin-tuc/giai-thuong-de-tai-noi-bat/wowtimes-nien-lich-thanh-tuu-viet-nam-2022-tan-hue-vien-37-nam-dua-thuong-hieu-dac-san-banh-pia-soc-trang-vuon-tam-trong-nuoc-va-quoc-te" target="_blank">Viện Kỷ Kỷ Lục Việt Nam</a>[cite: 7]</li>
                    <li>Tân Huê Viên xác lập kỷ kỷ kỷ kỷ kỷ kỷ kỷ kỷ kỷ lục bánh pía 368 kg năm 2026 – Viện Kỷ kỷ kỷ kỷ kỷ kỷ kỷ kỷ kỷ lục Việt Nam: <a href="https://vienkyluc.vn/tin-tuc/ban-quyen-tai-san-so/tan-hue-vien-lien-hoa-bao-thap" target="_blank">https://vienkyluc.vn/tin-tuc/ban-quyen-tai-san-so/tan-hue-vien-lien-hoa-bao-thap</a>[cite: 7]</li>
                </ul>
            </div>
        </main> 
        <!-- CỘT BÊN PHẢI (SIDEBAR): TÁC GIẢ VÀ ĐĂNG NHẬP -->
        <aside>
            <div class="sidebar-card" id="tac-gia">
                <h3 class="sidebar-title">Thành Viên Nhóm</h3>
                <ul class="author-list">
                    <li><strong>Hưng Phú</strong> <span class="leader-tag">Trưởng nhóm</span></li>
                    <li>Thảo Vy</li>
                    <li>Ngọc Hương</li>
                    <li>Lý Thư</li>
                    <li>Gia Bảo</li>
                    <li>Hân Bùi</li>
                    <li>Xuân Mai</li>
                </ul>
            </div>

<div class="sidebar-card">
                <h3 class="sidebar-title">Đăng Nhập</h3>
                <form class="login-form" action="#" method="post" onsubmit="return false;">
                    <input type="text" placeholder="Tên đăng nhập" required>
                    <input type="password" placeholder="Mật khẩu" required>
                    <button type="submit">Đăng Nhập</button>
                </form>
            </div>
        </aside>
</div>
<!-- PHẦN CHÂN TRANG (FOOTER): NGUYÊN VĂN TỪ SƠ ĐỒ TRÊN BẢNG -->
    <footer>
        DS -> Lớp 12A2 -> THPT HOANG DIEU
    </footer>

</body>
</html>
