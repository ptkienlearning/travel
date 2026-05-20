# 🌏 Nhật ký lữ hành — Travel Blog

Blog du lịch cá nhân, miễn phí 100%, host trên GitHub Pages.

## Cấu trúc file

```
travel-blog/
├── index.html    ← Trang public (gallery chuyến đi)
├── admin.html    ← Dashboard quản lý (chạy local)
└── data.json     ← Dữ liệu tất cả chuyến đi
```

---

## 🚀 Deploy lên GitHub Pages (miễn phí)

### Lần đầu tiên

1. Tạo tài khoản tại [github.com](https://github.com)
2. Tạo repository mới → đặt tên (VD: `travel-blog`) → Public
3. Upload 3 file: `index.html`, `admin.html`, `data.json`
4. Vào **Settings → Pages** → Source: `Deploy from branch` → `main` → `/ (root)` → Save
5. Đợi ~1 phút → trang live tại: `https://username.github.io/travel-blog`

### Workflow hàng ngày

```bash
# Sau khi chỉnh sửa trong admin và tải data.json về:
git add data.json
git commit -m "Thêm chuyến đi mới"
git push
# Trang tự cập nhật trong vài phút ✓
```

---

## 📸 Lấy URL ảnh từ Google Photos

1. Mở [photos.google.com](https://photos.google.com)
2. Click ảnh → nhấn **Chia sẻ** → **Tạo liên kết**
3. Copy URL → dán vào admin

> **Lưu ý:** Nếu ảnh không hiển thị, dùng Google Drive:
> Upload ảnh → Share "Anyone with link" → Lấy file ID → URL: `https://drive.google.com/uc?id=FILE_ID`

---

## ✏️ Cách sử dụng Admin

1. Mở `admin.html` trực tiếp trong Chrome/Firefox (không cần server)
2. **Thêm chuyến đi**: Sidebar → "Thêm chuyến đi" → điền thông tin → Lưu
3. **Cài đặt**: Đổi tên trang, bio, avatar
4. **Xuất dữ liệu**: Sidebar → "Xuất / Lưu dữ liệu" → Tải xuống data.json
5. Thay thế `data.json` cũ trong repo → Push lên GitHub

---

## 💡 Tips

- Dữ liệu được lưu tạm trong `localStorage` khi dùng admin → luôn export ra `data.json` trước khi đóng
- Nhập data.json cũ: Sidebar footer → "Tải data.json lên"
- Ảnh featured (nổi bật) hiển thị to hơn trên trang chủ
- Tags giúp lọc chuyến đi theo chủ đề

---

*Made with ❤ — Chi phí: 0đ/tháng*
