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
        }

        /* PHẦN ĐẦU: GIỚI THIỆU & THANH ĐIỀU HƯỚNG */
        header {
            background: linear-gradient(rgba(92, 14, 14, 0.9), rgba(139, 21, 21, 0.9)), url('anh-1.jpg') center/cover;
            color: #fff;
            padding: 50px 20px;
            text-align: center;
            box-shadow: 0 4px 10px rgba(0,0,0,0.15);
        }

        header h1 {
            font-size: 2.8rem;
            margin-bottom: 15px;
            letter-spacing: 1.5px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }

        header h2 {
            font-size: 1.4rem;
            font-weight: 400;
            margin-bottom: 10px;
            color: #fde8cd;
        }

        header p.sub-intro {
            font-size: 1.1rem;
            max-width: 800px;
            margin: 0 auto;
            color: #f5f5f5;
            font-style: italic;
        }

        /* Thanh điều hướng */
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
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
            padding: 12px 20px;
        }

        nav ul li a {
            color: #fff;
            text-decoration: none;
            font-weight: 600;
            font-size: 0.95rem;
            padding: 6px 14px;
            border-radius: 4px;
            transition: all 0.3s ease;
        }

        nav ul li a:hover {
            background-color: var(--accent-color);
            color: #fff;
        }

        /* BỐ CỤC CHÍNH */
        .container {
            max-width: 1200px;
            margin: 30px auto;
            padding: 0 20px;
            display: grid;
            grid-template-columns: 2.5fr 1fr;
            gap: 30px;
        }

        /* PHẦN THÂN: NỘI DUNG VÀ HÌNH ẢNH */
        main {
            background: #fff;
            padding: 40px;
            border-radius: 12px;
            box-shadow: 0 3px 10px rgba(0,0,0,0.05);
        }

        .content-section {
            margin-bottom: 40px;
        }

        .content-section:last-child {
            margin-bottom: 0;
        }

        h2.section-heading {
            font-size: 1.8rem;
            color: var(--primary-color);
            border-left: 5px solid var(--accent-color);
            padding-left: 15px;
            margin-bottom: 20px;
        }

        p {
            margin-bottom: 15px;
            text-align: justify;
            font-size: 1.05rem;
        }

        ul.styled-list {
            margin-left: 25px;
            margin-bottom: 20px;
        }

        ul.styled-list li {
            margin-bottom: 10px;
            font-size: 1.05rem;
        }

        /* Khung chứa ảnh đặt ngay sau nội dung */
        .img-container {
            margin: 25px 0;
            text-align: center;
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
        }

        .img-caption {
            margin-top: 10px;
            font-size: 0.95rem;
            color: #666;
            font-style: italic;
        }

        /* CỘT BÊN PHẢI (SIDEBAR): TÁC GIẢ & ĐĂNG NHẬP */
        aside {
            display: flex;
            flex-direction: column;
            gap: 25px;
        }

        .sidebar-card {
            background: #fff;
            padding: 25px;
            border-radius: 12px;
            box-shadow: 0 3px 10px rgba(0,0,0,0.05);
            border-top: 4px solid var(--primary-color);
        }

        .sidebar-title {
            font-size: 1.25rem;
            color: var(--primary-color);
            margin-bottom: 15px;
            padding-bottom: 8px;
            border-bottom: 2px solid #eee;
        }

        .author-list {
            list-style: none;
        }

        .author-list li {
            padding: 10px 0;
            border-bottom: 1px dashed #e5e5e5;
            font-size: 1rem;
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
            font-size: 0.75rem;
            padding: 3px 8px;
            border-radius: 12px;
            font-weight: bold;
        }

        .login-form {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }

        .login-form input {
            padding: 12px;
            border: 1px solid #ccc;
            border-radius: 6px;
            font-size: 1rem;
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
            padding: 12px;
            border-radius: 6px;
            font-weight: bold;
            font-size: 1rem;
            cursor: pointer;
            transition: background 0.3s;
        }

        .login-form button:hover {
            background-color: var(--primary-dark);
        }

        /* TÀI LIỆU THAM KHẢO */
        .references {
