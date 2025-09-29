<html lang="vi">
<head>
  <meta charset="UTF-8">
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #fef6f6; /* pastel hồng nhạt */
      margin: 0;
      padding: 20px;
      color: #333;
    }
    h1 {
      text-align: center;
      color: #ff6f61;
    }
    .menu {
      display: flex;
      justify-content: center;
      gap: 20px;
      margin: 20px 0;
    }
    .menu button {
      background-color: #a8dadc;
      border: none;
      padding: 10px 20px;
      font-size: 16px;
      border-radius: 8px;
      cursor: pointer;
      transition: 0.3s;
    }
    .menu button:hover {
      background-color: #457b9d;
      color: white;
    }
    .content {
      display: none;
      background: #fff;
      border-radius: 10px;
      padding: 20px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
      margin-top: 20px;
      line-height: 1.6;
    }
    .content.show {
      display: block;
    }
  </style>
</head>
<body>
  <div class="menu">
    <button onclick="showContent('lythuyet')">Lý thuyết cơ bản</button>
    <button onclick="showContent('vidu')">Ví dụ</button>
  </div>

  <!-- Nội dung mục Lý thuyết -->
  <div id="lythuyet" class="content">
    <h2>1. Thiết kế web là gì?</h2>
    <p>Thiết kế web là quá trình tạo ra giao diện và cấu trúc của một trang web để hiển thị trên trình duyệt, bao gồm:</p>
    <ul>
      <li>Nội dung (text, hình ảnh, video…)</li>
      <li>Giao diện (bố cục, màu sắc, font chữ…)</li>
      <li>Tương tác (nút bấm, form, liên kết…)</li>
    </ul>

    <h2>2. HTML là gì?</h2>
    <p>HTML (HyperText Markup Language) là ngôn ngữ đánh dấu, dùng để xây dựng cấu trúc cơ bản của trang web.</p>
    <p>HTML không phải ngôn ngữ lập trình, mà là khung xương của website.</p>

    <h2>3. Cấu trúc cơ bản của một trang HTML</h2>
    <pre>
&lt;!DOCTYPE html&gt;
&lt;html&gt;
&lt;head&gt;
    &lt;title&gt;Tiêu đề trang&lt;/title&gt;
&lt;/head&gt;
&lt;body&gt;
    &lt;h1&gt;Tiêu đề chính&lt;/h1&gt;
    &lt;p&gt;Đoạn văn bản nội dung.&lt;/p&gt;
&lt;/body&gt;
&lt;/html&gt;
    </pre>

    <h2>4. Một số thẻ HTML cơ bản</h2>
    <ul>
      <li>Tiêu đề: <code>&lt;h1&gt;...&lt;/h1&gt;</code></li>
      <li>Đoạn văn: <code>&lt;p&gt;...&lt;/p&gt;</code></li>
      <li>Liên kết: <code>&lt;a href="url"&gt;...&lt;/a&gt;</code></li>
      <li>Hình ảnh: <code>&lt;img src="link" alt="mô tả"&gt;</code></li>
      <li>Danh sách: <code>&lt;ul&gt;&lt;li&gt;...&lt;/li&gt;&lt;/ul&gt;</code></li>
      <li>Bảng: <code>&lt;table&gt;&lt;tr&gt;&lt;td&gt;&lt;/td&gt;&lt;/tr&gt;&lt;/table&gt;</code></li>
      <li>Form: <code>&lt;form&gt;&lt;input&gt;&lt;/form&gt;</code></li>
    </ul>

    <h2>5. Liên kết HTML với CSS và JS</h2>
    <ul>
      <li>CSS: Trang trí, định dạng</li>
      <li>JavaScript: Tương tác, hiệu ứng</li>
    </ul>
  </div>

  <!-- Nội dung mục Ví dụ -->
  <div id="vidu" class="content">
    <h2>1. Website của VnExpress cung cấp dịch vụ gì?</h2>
    <p>Chủ yếu cung cấp tin tức trực tuyến: chính trị, kinh tế, xã hội, thể thao, giải trí, công nghệ, du lịch…</p>
    <p>Dịch vụ kèm theo: quảng cáo, chuyên trang doanh nghiệp, rao vặt, việc làm, đọc báo có trả phí...</p>

    <h2>2. Đối tượng chính là ai?</h2>
    <ul>
      <li>Người đọc phổ thông</li>
      <li>Doanh nghiệp, tổ chức</li>
      <li>Học sinh, sinh viên, nhà nghiên cứu</li>
    </ul>

    <h2>3. Web có dạng Website hay Ứng dụng Web?</h2>
    <p>VnExpress.vn là Website tin tức dạng portal/news site.</p>
    <p>Song song có cả ứng dụng web + app trên iOS/Android.</p>
  </div>

  <script>
    function showContent(id) {
      document.querySelectorAll('.content').forEach(div => {
        div.classList.remove('show');
      });
      document.getElementById(id).classList.add('show');
    }
  </script>
</body>
</html>
