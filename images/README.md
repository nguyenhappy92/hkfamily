# 📸 Folder Images - HK Family

Đây là folder chứa tất cả ảnh cho website HK Family.

## 📁 Cấu trúc thư mục

```
images/
├── README.md              # File hướng dẫn này
├── hero/                  # Ảnh cho phần hero/banner
│   └── family-hero.jpg    # Ảnh nền hero section
├── members/               # Ảnh thành viên gia đình
│   ├── happy.jpg          # Ảnh của Happy
│   └── kieu.jpg           # Ảnh của Kiều
├── gallery/               # Album ảnh gia đình
│   ├── wedding/           # Ảnh cưới
│   ├── travel/            # Ảnh du lịch
│   └── daily/             # Ảnh hàng ngày
└── about/                 # Ảnh cho phần giới thiệu
    └── family-about.jpg   # Ảnh gia đình cho About section
```

## 🖼️ Kích thước ảnh khuyến nghị

### Hero Section (1920x1080px)
- **Mục đích:** Ảnh nền cho trang chủ
- **Kích thước:** 1920x1080px (Full HD)
- **Format:** JPG/WebP
- **Dung lượng:** < 500KB

### Member Photos (400x400px)
- **Mục đích:** Avatar thành viên gia đình
- **Kích thước:** 400x400px (vuông)
- **Format:** JPG/PNG
- **Dung lượng:** < 100KB

### Gallery Photos (800x600px)
- **Mục đích:** Album ảnh gia đình
- **Kích thước:** 800x600px (4:3)
- **Format:** JPG/WebP
- **Dung lượng:** < 200KB

### About Photo (600x400px)
- **Mục đích:** Ảnh cho phần giới thiệu
- **Kích thước:** 600x400px (3:2)
- **Format:** JPG/WebP
- **Dung lượng:** < 150KB

## 📝 Cách sử dụng

### 1. Upload ảnh vào folder tương ứng
- Drag & drop ảnh vào VS Code
- Hoặc copy/paste ảnh vào folder

### 2. Cập nhật code HTML/CSS
Thay thế các placeholder hiện tại:

#### Hero Background:
```css
.hero-background {
    background-image: url('../images/hero/family-hero.jpg');
    background-size: cover;
    background-position: center;
}
```

#### Member Avatars:
```css
.member-card:nth-child(1) .member-avatar {
    background-image: url('../images/members/happy.jpg');
    background-size: cover;
    background-position: center;
}

.member-card:nth-child(2) .member-avatar {
    background-image: url('../images/members/kieu.jpg');
    background-size: cover;
    background-position: center;
}
```

#### Gallery Items:
```css
.gallery-item:nth-child(1) .gallery-placeholder {
    background-image: url('../images/gallery/photo-1.jpg');
    background-size: cover;
    background-position: center;
}
```

#### About Section:
```css
.image-placeholder {
    background-image: url('../images/about/family-about.jpg');
    background-size: cover;
    background-position: center;
}
```

## 🎨 Tips tối ưu ảnh

### 1. Compress ảnh trước khi upload
- Sử dụng tools online: TinyPNG, Squoosh
- Giữ chất lượng tốt nhưng giảm dung lượng

### 2. Sử dụng format phù hợp
- **JPG:** Cho ảnh có nhiều màu (photos)
- **PNG:** Cho ảnh có nền trong suốt
- **WebP:** Format hiện đại, nhẹ hơn

### 3. Responsive images
Tạo nhiều kích thước cho responsive:
```
hero-desktop.jpg    (1920x1080)
hero-tablet.jpg     (1024x768)
hero-mobile.jpg     (480x320)
```

## 🚀 Sau khi upload ảnh

1. **Test local:** Mở index.html để xem ảnh
2. **Commit & Push:**
   ```bash
   git add images/
   git commit -m "📸 Add family photos"
   git push origin main
   ```
3. **Deploy:** GitHub Pages sẽ tự động cập nhật

## 🔧 Troubleshooting

### Ảnh không hiển thị?
- Kiểm tra đường dẫn file
- Đảm bảo tên file không có ký tự đặc biệt
- File extension phải đúng (.jpg, .png, .webp)

### Ảnh load chậm?
- Compress ảnh nhỏ hơn
- Sử dụng format WebP
- Thêm lazy loading

---

**Happy uploading! 📸✨**