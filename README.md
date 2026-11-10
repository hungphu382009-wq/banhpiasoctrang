# banhpiasoctrang
index.html
<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>PIA HOUSE | Đặc sản bánh pía Sóc Trăng</title>
<style>
*{margin:0;padding:0;box-sizing:border-box}
body{font-family:Arial,sans-serif;background:#f8f2e8;color:#493323}
header{background:#503522;color:#fff;padding:22px 8%;display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;gap:15px}
.logo{font-size:27px;font-weight:bold;letter-spacing:3px;color:#f0d4a1}
nav a{color:white;text-decoration:none;margin-left:20px;font-size:14px}
.hero{padding:75px 8%;display:flex;align-items:center;justify-content:space-between;gap:35px;flex-wrap:wrap;background:#eee0ca}
.hero-text{flex:1;min-width:260px}
.hero h1{font-size:48px;color:#503522;margin-bottom:20px}
.hero p{font-size:18px;line-height:1.7;margin-bottom:25px}
.hero img{width:100%;max-width:440px;border-radius:18px;object-fit:cover}
.btn{display:inline-block;background:#9c6b36;color:white;padding:13px 25px;border-radius:30px;text-decoration:none}
section{padding:65px 8%}
.heading{text-align:center;font-size:32px;color:#69452b;margin-bottom:35px}
.products{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:25px}
.product{background:white;border-radius:15px;overflow:hidden;box-shadow:0 4px 15px #00000012;padding-bottom:22px;text-align:center}
.product img{width:100%;height:190px;object-fit:cover}
.product h3{margin:18px 8px 10px}
.product p{color:#95642f;margin-bottom:15px}
.about{text-align:center;background:#eee0ca;line-height:1.9}
.about p{max-width:750px;margin:auto}
footer{background:#503522;color:white;text-align:center;padding:30px;line-height:2}
@media(max-width:600px){.hero h1{font-size:36px}nav a{margin:5px;font-size:13px}}
</style>
</head>
<body>
<header>
<div class="logo">PIA HOUSE</div>
<nav>
<a href="#home">Trang chủ</a>
<a href="#products">Sản phẩm</a>
<a href="#about">Về chúng tôi</a>
</nav>
</header>

<div class="hero" id="home">
<div class="hero-text">
<h1>Hương vị quê nhà</h1>
<p>PIA HOUSE mang đến những chiếc bánh pía Sóc Trăng thơm ngon, đậm đà hương vị truyền thống.</p>
<a class="btn" href="#products">Khám phá sản phẩm</a>
</div>
<img src="https://images.unsplash.com/photo-1558961363-fa8fdf82db35?w=900" alt="Bánh ngọt">
</div>

<section id="products">
<h2 class="heading">Sản phẩm nổi bật</h2>
<div class="products">
<div class="product">
<img src="https://images.unsplash.com/photo-1578985545062-69928b1d9587?w=600" alt="Bánh pía">
<h3>Bánh pía truyền thống</h3>
<p>Giá: 45.000đ / hộp</p>
<a class="btn" href="#contact">Đặt hàng</a>
</div>
<div class="product">
<img src="https://images.unsplash.com/photo-1606313564200-e75d5e30476c?w=600" alt="Bánh">
<h3>Bánh pía đậu xanh</h3>
<p>Giá: 50.000đ / hộp</p>
<a class="btn" href="#contact">Đặt hàng</a>
</div>
<div class="product">
<img src="https://images.unsplash.com/photo-1486427944299-d1955d23e34d?w=600" alt="Bánh ngọt">
<h3>Bánh pía sầu riêng</h3>
<p>Giá: 55.000đ / hộp</p>
<a class="btn" href="#contact">Đặt hàng</a>
</div>
</div>
</section>

<section class="about" id="about">
<h2 class="heading">Câu chuyện PIA HOUSE</h2>
<p>Từ vùng đất Sóc Trăng giàu truyền thống, bánh pía đã trở thành một đặc sản gắn liền với văn hóa ẩm thực miền Tây. PIA HOUSE mong muốn lan tỏa hương vị thân quen ấy bằng một phong cách gần gũi, chỉn chu và hiện đại.</p>
</section>

<section id="contact">
<h2 class="heading">Đặt bánh cùng PIA HOUSE</h2>
<p style="text-align:center;line-height:2">Bạn yêu thích bánh pía Sóc Trăng? Hãy liên hệ với chúng tôi để được tư vấn và đặt hàng nhé!</p>
<p style="text-align:center;margin-top:20px"><a class="btn" href="https://zalo.me/" target="_blank">Liên hệ qua Zalo</a></p>
</section>

<footer>
<strong>PIA HOUSE</strong>
<p>Đậm vị quê hương – Trọn tình đặc sản</p>
<p>Đặc sản bánh pía Sóc Trăng</p>
</footer>
</body>
</html>
