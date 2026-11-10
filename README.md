# banhpiasoctrang
index.html
<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Bánh Pía Sóc Trăng – Nhà Làm Thủ Công</title>
<meta name="description" content="Bánh pía Sóc Trăng làm thủ công: đậu xanh sầu riêng trứng muối, khoai môn, lá dứa. Đặt hàng online, giao toàn quốc.">
<link rel="icon" href="data:,">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Be+Vietnam+Pro:wght@400;500;600&family=Fraunces:opsz,wght@9..144,600;9..144,800&display=swap" rel="stylesheet">
<style>
:root{
  --bean:#EEF0D2;
  --leaf:#2F5D3A;
  --yolk:#F2B632;
  --crust:#FBF6E4;
  --ink:#2B2118;
  --line:#CFD4A6;
  --r:14px;
}
*{box-sizing:border-box;margin:0}
html{scroll-behavior:smooth;scroll-padding-top:72px}
body{font-family:"Be Vietnam Pro",system-ui,sans-serif;background:var(--bean);color:var(--ink);line-height:1.65}
h1,h2,h3{font-family:Fraunces,Georgia,serif;line-height:1.15}
a{color:inherit}
:focus-visible{outline:3px solid var(--leaf);outline-offset:3px}
.wrap{max-width:1080px;margin:0 auto;padding:0 20px}
section{padding:72px 0}

header{position:sticky;top:0;z-index:10;background:var(--leaf);color:var(--crust)}
header .wrap{display:flex;align-items:center;justify-content:space-between;height:60px}
.logo{font-family:Fraunces,serif;font-weight:800;font-size:1.25rem;text-decoration:none}
nav{display:flex;gap:20px;align-items:center;font-size:.95rem}
nav a{text-decoration:none}
nav a:hover{text-decoration:underline}
.cart-btn{background:var(--yolk);color:var(--ink);border:0;border-radius:99px;padding:7px 16px;font-family:inherit;font-size:.9rem;font-weight:600;cursor:pointer}

.hero{padding:56px 0 72px}
.hero .wrap{display:grid;grid-template-columns:1.1fr .9fr;gap:40px;align-items:center}
.hero h1{font-size:clamp(2.2rem,5.5vw,3.8rem);font-weight:800;color:var(--leaf)}
.lead{margin:18px 0 28px;max-width:46ch;font-size:1.05rem}
.actions{display:flex;flex-wrap:wrap;gap:12px}
.btn{display:inline-block;background:var(--leaf);color:var(--crust);padding:13px 26px;border-radius:99px;text-decoration:none;font-weight:600;border:2px solid var(--leaf);cursor:pointer;font-family:inherit;font-size:1rem}
.btn:hover{background:#244a2d}
.btn.alt{background:transparent;color:var(--leaf)}
.btn.alt:hover{background:rgba(47,93,58,.1)}

.pia-wrap{display:grid;place-items:center}
.pia{
  width:min(100%,360px);aspect-ratio:1;border-radius:50%;
  background:
    radial-gradient(circle closest-side,var(--yolk) 0 22%,#E39A1B 22% 26%,#A9B455 26% 70%,#8F9C45 70% 74%,transparent 74%),
    repeating-radial-gradient(circle closest-side,#FBF1D0 0 5px,#EBD08F 5px 7px,#FDF8E6 7px 12px);
  box-shadow:0 0 0 6px var(--crust),0 18px 40px rgba(47,93,58,.25);
}
.pia-cap{margin-top:22px;font-size:.9rem;text-align:center;max-width:32ch}

.sec-head{max-width:56ch;margin-bottom:36px}
.sec-head h2{font-size:clamp(1.7rem,3.5vw,2.4rem);color:var(--leaf)}
.sec-head p{margin-top:10px}
.grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(250px,1fr));gap:20px}
.card{background:var(--crust);border-radius:var(--r);padding:22px;display:flex;flex-direction:column;border-left:8px solid var(--c,var(--leaf))}
.card h3{font-size:1.25rem}
.card .desc{margin:8px 0 16px;font-size:.93rem;flex:1}
.card .row{display:flex;align-items:center;justify-content:space-between;gap:10px;flex-wrap:wrap}
.price{font-weight:600;font-size:1.05rem}
.price small{font-weight:400;opacity:.7}
.add{background:var(--ink);color:var(--crust);border:0;border-radius:99px;padding:9px 18px;font-family:inherit;font-size:.9rem;font-weight:500;cursor:pointer}
.add:hover{background:var(--leaf)}

.story{background:var(--leaf);color:var(--crust)}
.story h2{font-size:clamp(1.7rem,3.5vw,2.4rem);margin-bottom:28px}
.story .cols{display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:32px}
.story h3{font-size:1.15rem;color:var(--yolk);margi
