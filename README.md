# 🏠 HK Family Website

Chào mừng đến với website gia đình HK Family! Đây là một website đẹp mắt, hiện đại được thiết kế để chia sẻ những khoảnh khắc đẹp và câu chuyện của gia đình bạn.

## ✨ Tính năng

- **Thiết kế responsive** - Hoạt động hoàn hảo trên tất cả thiết bị
- **Animations mượt mà** - Hiệu ứng chuyển động đẹp mắt
- **Hero section ấn tượng** - Trang chủ thu hút với gradient và hiệu ứng
- **Gallery ảnh** - Trưng bày album ảnh gia đình
- **Timeline** - Dòng thời gian các sự kiện quan trọng
- **Form liên hệ** - Cho phép người khác liên hệ với gia đình
- **Hiệu ứng đặc biệt** - Tim bay, scroll indicator, typing effect

## 🚀 Cách triển khai lên GitHub Pages

### Bước 1: Commit và push code
```bash
git add .
git commit -m "🎉 Add HK Family website"
git push origin main
```

### Bước 2: Kích hoạt GitHub Pages
1. Vào repository trên GitHub
2. Vào **Settings** > **Pages**
3. Trong **Source**, chọn **Deploy from a branch**
4. Chọn branch **main** và folder **/ (root)**
5. Click **Save**

Website sẽ có địa chỉ: `https://nguyenhappy92.github.io/hkfamily`

## 🎨 Tùy chỉnh website

### Thay đổi thông tin gia đình

1. **Tên gia đình**: Sửa trong `index.html` tất cả các chỗ "HK Family"
2. **Thành viên**: Sửa section `#members` để thêm/bớt/đổi thông tin thành viên
3. **Timeline**: Cập nhật section `#timeline` với các sự kiện của gia đình bạn
4. **Thông tin liên hệ**: Sửa section `#contact` với email, số điện thoại thật

### Thêm ảnh thật

Thay thế các placeholder bằng ảnh thật:

1. Tạo folder `images/` trong project
2. Thêm ảnh vào folder này
3. Sửa CSS để thay `background` của `.image-placeholder` và `.gallery-placeholder`:

```css
/* Ví dụ cho ảnh hero */
.hero-background {
    background-image: url('images/family-hero.jpg');
    background-size: cover;
    background-position: center;
}

/* Ví dụ cho gallery */
.gallery-item:nth-child(1) .gallery-placeholder {
    background-image: url('images/family-1.jpg');
    background-size: cover;
    background-position: center;
}
```

### Thay đổi màu sắc

Màu chính của website được định nghĩa trong `style.css`. Tìm và thay đổi:

```css
/* Màu chính - gradient cam đỏ */
background: linear-gradient(45deg, #ff6b6b, #ffa500);

/* Màu phụ - gradient tím xanh */
background: linear-gradient(135deg, #667eea, #764ba2);
```

### Thêm mạng xã hội

Trong section footer, cập nhật các liên kết mạng xã hội:

```html
<div class="footer-social">
    <a href="https://facebook.com/your-page"><i class="fab fa-facebook"></i></a>
    <a href="https://instagram.com/your-account"><i class="fab fa-instagram"></i></a>
    <a href="https://youtube.com/your-channel"><i class="fab fa-youtube"></i></a>
</div>
```

## 📱 Tính năng di động

Website được tối ưu hoàn toàn cho mobile:
- Menu hamburger trên mobile
- Layout responsive
- Touch-friendly buttons
- Optimized images

## 🛠️ Cấu trúc file

```
hkfamily/
├── index.html          # Trang chính
├── style.css           # Stylesheet chính  
├── script.js           # JavaScript
├── README.md           # Hướng dẫn này
└── images/            # Folder chứa ảnh (tạo thêm)
```

## 🎯 Các section chính

1. **Hero** - Trang chủ với slogan
2. **About** - Giới thiệu gia đình
3. **Members** - Thành viên gia đình
4. **Gallery** - Album ảnh
5. **Timeline** - Dòng thời gian
6. **Contact** - Liên hệ
7. **Footer** - Thông tin cuối trang

## 🚀 Tối ưu hóa

### SEO
- Thêm meta description trong `<head>`
- Thêm Open Graph tags cho social sharing
- Optimize ảnh với alt text

### Performance
- Compress ảnh trước khi upload
- Sử dụng WebP format cho ảnh
- Minify CSS/JS cho production

## 💡 Gợi ý mở rộng

1. **Blog section** - Chia sẻ câu chuyện gia đình
2. **Recipe section** - Các món ăn đặc trưng
3. **Events calendar** - Lịch sự kiện gia đình
4. **Guest book** - Sổ lưu bút cho khách
5. **Multi-language** - Hỗ trợ nhiều ngôn ngữ

## 🔧 Troubleshooting

### Website không hiển thị trên GitHub Pages
- Kiểm tra file `index.html` có đúng tên không
- Đảm bảo đã commit và push code
- Chờ 5-10 phút để GitHub Pages deploy

### Ảnh không hiển thị
- Kiểm tra đường dẫn ảnh
- Đảm bảo ảnh đã được commit và push
- Sử dụng đường dẫn tương đối

### CSS/JS không hoạt động
- Kiểm tra console browser (F12) để xem lỗi
- Đảm bảo đường dẫn file đúng
- Clear cache browser

## 📞 Hỗ trợ

Nếu cần hỗ trợ thêm, bạn có thể:
- Tạo issue trong GitHub repository
- Tham khảo documentation của GitHub Pages
- Học thêm HTML/CSS/JavaScript basics

---

**Made with ❤️ for HK Family**

*Chúc gia đình bạn luôn hạnh phúc và website thành công!* 🎉