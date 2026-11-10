
index.html
<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Bánh Pía Sóc Trăng – Đặt bánh online</title>
<meta name="description" content="Bánh pía Sóc Trăng làm thủ công. Chọn vị bánh, đặt hàng online qua Zalo, giao toàn quốc.">
<meta name="theme-color" content="#9B1C1F">
<link rel="icon" href="data:,">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Bitter:wght@600;800&family=Lexend:wght@400;500;600&display=swap" rel="stylesheet">
<style>
:root{--red:#9B1C1F;--red-d:#7A1417;--gold:#E9B949;--gold-l:#FBEFC9;--paper:#FFFDF8;--ink:#2A1410;--mute:#6B5A52;--rule:#E6D8B8}
*{box-sizing:border-box}
body,h1,h2,h3,p,ul,ol{margin:0}
ul,ol{padding:0;list-style:none}
html{scroll-behavior:smooth;scroll-padding-top:70px}
body{font-family:Lexend,system-ui,sans-serif;background:var(--paper);color:var(--ink);line-height:1.7;padding-bottom:84px}
h1,h2,h3{font-family:Bitter,Georgia,serif;line-height:1.2}
a{color:inherit}
:focus-visible{outline:3px solid var(--gold);outline-offset:3px}
.wrap{max-width:1040px;margin:0 auto;padding:0 20px}
section{padding:68px 0}
h2{font-size:clamp(1.7rem,3.6vw,2.4rem);color:var(--red);font-weight:800}
.sub{margin-top:8px;color:var(--mute);max-width:56ch}

.top{position:sticky;top:0;z-index:15;background:var(--red-d);color:var(--gold-l)}
.top .wrap{display:flex;align-items:center;justify-content:space-between;height:56px;gap:12px}
.brand{font-family:Bitter,serif;font-weight:800;font-size:1.2rem;text-decoration:none}
.btn{display:inline-block;border:0;border-radius:8px;padding:12px 22px;background:var(--gold);color:var(--ink);font-family:inherit;font-size:1rem;font-weight:600;text-decoration:none;cursor:pointer}
.btn:hover{background:#f3c862}
.btn.red{background:var(--red);color:#fff}
.btn.red:hover{background:var(--red-d)}
.btn.sm{padding:8px 16px;font-size:.9rem}

.hero{background:var(--red);color:#fff;padding:60px 0 76px}
.hero .wrap{display:grid;grid-template-columns:1.1fr .9fr;gap:40px;align-items:center}
.hero h1{font-size:clamp(2.2rem,5.4vw,3.8rem);font-weight:800}
.lead{margin:18px 0 28px;max-width:44ch;font-size:1.05rem;color:var(--gold-l)}
.trio{position:relative;width:100%;max-width:400px;aspect-ratio:1.1;margin:0 auto}
.pia{position:absolute;aspect-ratio:1;border-radius:50%;
  background:radial-gradient(circle closest-side,var(--core) 0 20%,var(--fill) 20% 68%,transparent 68%),
  repeating-radial-gradient(circle closest-side,#FBF1D0 0 5px,#EBD08F 5px 7px,#FDF8E6 7px 12px);
  box-shadow:0 10px 24px rgba(0,0,0,.35),0 0 0 4px #fff}
.p1{width:62%;left:0;top:10%;--fill:#A9B455;--core:#F2B632}
.p2{width:54%;right:0;top:0;--fill:#8E6BB0;--core:#F2B632}
.p3{width:48%;left:30%;bottom:0;--fill:#5E9A55;--core:#FFF3C4}
.trio-cap{margin-top:16px;text-align:center;font-size:.88rem;color:var(--gold-l)}

.menu{margin-top:30px}
.dish{padding:18px 0;border-bottom:1px solid var(--rule)}
.dish-top{display:flex;align-items:baseline;gap:10px}
.dish h3{font-size:1.2rem}
.dots{flex:1;border-bottom:2px dotted #C9B27A;min-width:20px;transform:translateY(-4px)}
.price{font-weight:600;white-space:nowrap}
.dish-bot{display:flex;justify-content:space-between;align-items:center;gap:16px;margin-top:6px}
.desc{color:var(--mute);font-size:.93rem;max-width:52ch}
.step{display:flex;align-items:center;gap:6px;flex-shrink:0}
.step button{width:36px;height:36px;border:1.5px solid var(--ink);border-radius:8px;background:#fff;font-size:1.1rem;line-height:1;cursor:pointer}
.step button:hover{background:var(--gold)}
.step span{min-width:26px;text-align:center;font-weight:600}
.unit{font-size:.85rem;color:var(--mute);margin-top:14px}

.band{background:var(--gold-l)}
.facts{display:grid;grid-template-columns:repeat(auto-fit,minmax(230px,1fr));gap:28px;margin-top:28px}
.facts div{border-top:4px solid var(--red);padding-top:12px}
.facts h3{font-size:1.1rem;margin-bottom:6px}
.steps{margin-top:28px;counter-reset:s;display:grid;gap:18px;max-width:640px}
.steps li{counter-increment:s;display:grid;grid-template-columns:48px 1fr;gap:14px;align-items:start}
.steps li::before{content:counter(s);width:48px;height:48px;border-radius:50%;background:var(--red);color:#fff;display:grid;place-items:center;font-family:Bitter,serif;font-weight:800;font-size:1.3rem}
.steps b{display:block}
details{border-bottom:1px solid var(--rule);padding:14px 0;max-width:720px}
summary{cursor:pointer;font-weight:600}
details p{margin-top:8px;color:var(--mute)}

footer{background:var(--ink);color:var(--gold-l);padding:34px 0;font-size:.92rem}
footer .wrap{display:flex;flex-wrap:wrap;gap:20px;justify-content:space-between}

.bar{position:fixed;left:0;right:0;bottom:0;z-index:20;background:var(--ink);color:#fff;padding:12px 20px;display:flex;justify-content:space-between;align-items:center;gap:12px}
.bar[hidden]{display:none}
dialog{border:0;border-radius:14px;padding:0;width:calc(100% - 24px);max-width:520px;max-height:calc(100vh - 24px);overflow:auto;background:var(--paper);color:var(--ink)}
dialog::backdrop{background:rgba(42,20,16,.6)}
.dlg{padding:24px}
.dlg-head{display:flex;justify-content:space-between;align-items:center;margin-bottom:10px}
.dlg h2{font-size:1.5rem}
.close{border:0;background:none;font:inherit;font-weight:600;cursor:pointer;text-decoration:underline}
.item{display:flex;justify-content:space-between;align-items:center;gap:12px;padding:10px 0;border-bottom:1px solid var(--rule)}
.item b{display:block;font-weight:600;font-size:.95rem}
.item small{color:var(--mute)}
.total{display:flex;justify-content:space-between;margin:14px 0 6px;font-size:1.1rem;font-weight:600}
label{display:block;font-size:.88rem;font-weight:500;margin:12px 0 4px}
input,textarea{width:100%;padding:11px 12px;border:1.5px solid #cdbf9b;border-radius:8px;font:inherit;background:#fff;color:var(--ink)}
#msg{margin-top:12px;font-weight:500;color:var(--red)}
#fallback{margin-top:10px}
.note{font-size:.82rem;color:var(--mute);margin-top:10px}

@media(max-width:780px){
  .hero .wrap{grid-template-columns:1fr}
  section{padding:48px 0}
  .dish-bot{align-items:flex-end}
}
@media(prefers-reduced-motion:reduce){html{scroll-behavior:auto}}
</style>
</head>
<body>

<header class="top">
  <div class="wrap">
    <a class="brand" href="#dau-trang" id="shopName">Bánh Pía Sóc Trăng</a>
    <a class="btn sm" href="#thuc-don">Xem thực đơn</a>
  </div>
</header>

<main id="dau-trang">
  <section class="hero">
    <div class="wrap">
      <div>
        <h1>Bánh pía Sóc Trăng, vỏ nhiều lớp, nhân bùi béo</h1>
        <p class="lead">Làm thủ công từ đậu xanh, sầu riêng, khoai môn và trứng muối. Chọn vị bạn thích, đặt qua Zalo, shop gửi bánh đến tận nhà.</p>
        <a class="btn" href="#thuc-don">Chọn bánh ngay</a>
      </div>
      <div>
        <div class="trio" role="img" aria-label="Ba chiếc bánh pía cắt đôi: nhân đậu xanh, khoai môn và lá dứa">
          <div class="pia p1"></div><div class="pia p2"></div><div class="pia p3"></div>
        </div>
        <p class="trio-cap">Đậu xanh, khoai môn và lá dứa: ba trong số các vị của shop.</p>
      </div>
    </div>
  </section>

  <section id="thuc-don">
    <div class="wrap">
      <h2>Thực đơn</h2>
      <p class="sub">Bấm dấu + để thêm bánh vào đơn. Giá tính theo hộp.</p>
      <ul class="menu" id="menu"></ul>
      <p class="unit" id="unitNote"></p>
    </div>
  </section>

  <section class="band">
    <div class="wrap">
      <h2>Vì sao bánh pía Sóc Trăng ngon?</h2>
      <div class="facts">
        <div><h3>Vỏ nhiều lớp</h3><p>Bột cán với dầu rồi gấp nhiều lần, nên vỏ mỏng, xốp và tách thành từng lớp khi cắn.</p></div>
        <div><h3>Nhân xào nhuyễn</h3><p>Đậu xanh hấp, xay mịn, xào dẻo cho thơm bùi, ngọt vừa phải.</p></div>
        <div><h3>Sầu riêng, trứng muối</h3><p>Sầu riêng béo thơm, lòng đỏ trứng muối mặn nhẹ, cân bằng vị ngọt của nhân.</p></div>
      </div>
    </div>
  </section>

  <section>
    <div class="wrap">
      <h2>Đặt hàng thế nào?</h2>
      <ol class="steps">
        <li><div><b>Chọn bánh</b>Thêm các vị bạn thích vào đơn ở phần thực đơn.</div></li>
        <li><div><b>Gửi đơn qua Zalo</b>Điền tên, số điện thoại, địa chỉ rồi bấm gửi. Đơn được sao chép sẵn để bạn dán vào Zalo.</div></li>
        <li><div><b>Nhận bánh</b>Shop xác nhận đơn, báo phí giao hàng và gửi bánh cho bạn.</div></li>
      </ol>
    </div>
  </section>

  <section class="band">
    <div class="wrap">
      <h2>Câu hỏi thường gặp</h2>
      <div style="margin-top:20px">
        <details><summary>Bảo quản bánh pía như thế nào?</summary><p>Để nơi khô ráo, thoáng mát, tránh nắng. Hạn dùng được ghi trên hộp. Mở hộp rồi nên dùng sớm để bánh giữ độ giòn.</p></details>
        <details><summary>Shop có giao hàng toàn quốc không?</summary><p>Có. Shop gửi qua đơn vị vận chuyển. Phí và thời gian giao sẽ được báo khi xác nhận đơn.</p></details>
        <details><summary>Mua làm quà tặng được không?</summary><p>Được. Bạn ghi chú "làm quà" trong địa chỉ nhận hàng, shop sẽ đóng hộp gọn gàng cho bạn.</p></details>
        <details><summary>Thanh toán bằng cách nào?</summary><p>Shop sẽ hướng dẫn cách thanh toán khi xác nhận đơn qua Zalo.</p></details>
      </div>
    </div>
  </section>
</main>

<footer>
  <div class="wrap">
    <div><b id="fName"></b><br><span id="fAddr"></span></div>
    <div>Zalo/Hotline: <a id="fTel" href="#"></a><br><span id="fHours"></span></div>
  </div>
</footer>

<div class="bar" id="bar" hidden>
  <span id="barText"></span>
  <button class="btn" id="openDlg" type="button">Xem đơn và đặt hàng</button>
</div>

<dialog id="dlg" aria-labelledby="dlgTitle">
  <div class="dlg">
    <div class="dlg-head"><h2 id="dlgTitle">Đơn của bạn</h2><button class="close" id="closeDlg" type="button">Đóng</button></div>
    <div id="dlgItems"></div>
    <label for="name">Họ tên</label>
    <input id="name" autocomplete="name">
    <label for="phone">Số điện thoại</label>
    <input id="phone" type="tel" autocomplete="tel">
    <label for="addr">Địa chỉ nhận hàng</label>
    <textarea id="addr" rows="3" autocomplete="street-address"></textarea>
    <p style="margin-top:18px"><button class="btn red" id="send" type="button">Gửi đơn qua Zalo</button></p>
    <p id="msg" role="status"></p>
    <textarea id="fallback" rows="7" readonly hidden aria-label="Nội dung đơn hàng để sao chép"></textarea>
    <p class="note">Đơn được sao chép tự động. Bạn chỉ cần dán vào khung chat Zalo của shop.</p>
  </div>
</dialog>

<script>
/* ====== CHỈNH SỬA THÔNG TIN SHOP TẠI ĐÂY ====== */
var SHOP = {
  name: "Bánh Pía Sóc Trăng",
  zalo: "0900000000",
  address: "123 Đường Trần Hưng Đạo, TP. Sóc Trăng",
  hours: "7:00 – 20:00 mỗi ngày"
};
var UNIT = "hộp 4 bánh";
var PRODUCTS = [
  {id:"sr", name:"Đậu xanh sầu riêng trứng muối", desc:"Béo thơm sầu riêng, bùi đậu xanh, mặn nhẹ trứng muối.", price:180000},
  {id:"dx", name:"Đậu xanh trứng muối",           desc:"Vị truyền thống, ngọt thanh, hợp người không ăn sầu riêng.", price:150000},
  {id:"ld", name:"Đậu xanh lá dứa",               desc:"Nhân xanh thơm mùi lá dứa, dẻo mịn, ít ngọt.", price:140000},
  {id:"km", name:"Khoai môn trứng muối",          desc:"Khoai môn nghiền mịn, thơm bùi, có lòng đỏ trứng muối.", price:160000},
  {id:"tc", name:"Thập cẩm",                      desc:"Hạt dưa, lạp xưởng, trứng muối, đậu xanh. Đậm đà, nhiều vị.", price:170000},
  {id:"ch", name:"Bánh pía chay",                 desc:"Đậu xanh, khoai môn, không trứng, không mỡ. Hợp ngày chay.", price:130000}
];
/* =============================================== */

var cart = {};
var dlg = document.getElementById("dlg");
function $(s){ return document.querySelector(s); }
function fmt(n){ return new Intl.NumberFormat("vi-VN").format(n) + "đ"; }
function find(id){ return PRODUCTS.filter(function(p){ return p.id === id; })[0]; }

function stepHTML(p){
  return '<div class="step">' +
    '<button type="button" aria-label="Giảm ' + p.name + '" data-id="' + p.id + '" data-d="-1">−</button>' +
    '<span data-qty="' + p.id + '">' + (cart[p.id] || 0) + '</span>' +
    '<button type="button" aria-label="Thêm ' + p.name + '" data-id="' + p.id + '" data-d="1">+</button></div>';
}

function calc(){
  var count = 0, total = 0, lines = [];
  Object.keys(cart).forEach(function(id){
    var p = find(id);
    count += cart[id];
    total += p.price * cart[id];
    lines.push({p:p, q:cart[id]});
  });
  return {count:count, total:total, lines:lines};
}

function change(id, d){
  cart[id] = (cart[id] || 0) + d;
  if (cart[id] <= 0) delete cart[id];
  sync();
}

function sync(){
  var c = calc();
  PRODUCTS.forEach(function(p){
    document.querySelectorAll('#menu [data-qty="' + p.id + '"]').forEach(function(el){ el.textContent = cart[p.id] || 0; });
  });
  $("#bar").hidden = c.count === 0;
  $("#barText").textContent = c.count + " hộp, tạm tính " + fmt(c.total);
  $("#dlgItems").innerHTML = c.lines.map(function(l){
    return '<div class="item"><div><b>' + l.p.name + '</b><small>' + fmt(l.p.price) + ' / ' + UNIT + '</small></div>' + stepHTML(l.p) + '</div>';
  }).join("") + '<div class="total"><span>Tạm tính</span><span>' + fmt(c.total) + '</span></div>';
  if (c.count === 0 && dlg.open) dlg.close();
}

$("#menu").innerHTML = PRODUCTS.map(function(p){
  return '<li class="dish"><div class="dish-top"><h3>' + p.name + '</h3><span class="dots"></span><span class="price">' + fmt(p.price) + '</span></div>' +
    '<div class="dish-bot"><p class="desc">' + p.desc + '</p>' + stepHTML(p) + '</div></li>';
}).join("");
$("#unitNote").textContent = "Giá tính theo " + UNIT + ". Phí giao hàng được báo khi xác nhận đơn.";

$("#shopName").textContent = SHOP.name;
$("#fName").textContent = SHOP.name;
$("#fAddr").textContent = "Địa chỉ: " + SHOP.address;
$("#fHours").textContent = "Mở cửa: " + SHOP.hours;
$("#fTel").textContent = SHOP.zalo;
$("#fTel").href = "tel:" + SHOP.zalo;

document.addEventListener("click", function(e){
  var b = e.target.closest ? e.target.closest("button[data-id]") : null;
  if (b) change(b.getAttribute("data-id"), Number(b.getAttribute("data-d")));
});
$("#openDlg").addEventListener("click", function(){ dlg.showModal(); });
$("#closeDlg").addEventListener("click", function(){ dlg.close(); });
dlg.addEventListener("click", function(e){ if (e.target === dlg) dlg.close(); });

function copyText(t){
  try {
    return navigator.clipboard.writeText(t).then(function(){ return true; }, function(){ return false; });
  } catch (err) {
    return Promise.resolve(false);
  }
}

$("#send").addEventListener("click", function(){
  var msg = $("#msg"), box = $("#fallback");
  var name = $("#name").value.trim(), phone = $("#phone").value.trim(), addr = $("#addr").value.trim();
  var c = calc();
  box.hidden = true;

  if (!c.count){ msg.textContent = "Đơn đang trống. Hãy thêm ít nhất 1 hộp bánh."; return; }
  if (!name || !phone || !addr){ msg.textContent = "Vui lòng điền đủ họ tên, số điện thoại và địa chỉ."; return; }
  if (!/^(0\d{9}|\+84\d{9})$/.test(phone.replace(/[\s.\-]/g, ""))){
    msg.textContent = "Số điện thoại chưa đúng. Hãy nhập 10 số, ví dụ 0912345678."; return;
  }

  var text = "ĐƠN HÀNG BÁNH PÍA\n" +
    c.lines.map(function(l){ return "- " + l.p.name + " x " + l.q + " hộp"; }).join("\n") +
    "\nTạm tính: " + fmt(c.total) + "\nNgười nhận: " + name + "\nSĐT: " + phone + "\nĐịa chỉ: " + addr;

  window.open("https://zalo.me/" + SHOP.zalo, "_blank", "noopener");
  copyText(text).then(function(ok){
    if (ok){
      msg.textContent = "Đã sao chép đơn hàng. Dán vào Zalo để gửi cho shop.";
    } else {
      msg.textContent = "Chưa tự sao chép được. Hãy chép nội dung bên dưới rồi dán vào Zalo.";
      box.value = text; box.hidden = false; box.focus(); box.select();
    }
  });
});

sync();
</script>
</body>
</html>
