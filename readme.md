# WuysBio

WuysBio là một trang bio cá nhân hiện đại được lấy cảm hứng từ guns.lol, cho phép bạn hiển thị thông tin cá nhân, avatar, mạng xã hội, video background và trình phát nhạc với giao diện aesthetic và mượt mà.

![preview](./avatar.jpg)

---

## ✨ Features

* 🎥 Video background toàn màn hình
* 👤 Profile card với avatar và bio
* 🔗 Social media links (Facebook, TikTok, Roblox, Website, etc.)
* 🎵 Music player tích hợp (playlist + controls)
* 📊 Visitor counter (localStorage)
* 💳 Payment info + QR code
* 📱 Responsive (mobile + desktop)
* ⚡ Server nhẹ sử dụng Bun (stream video/mp3 mượt)

---

## 📁 Project Structure

```
WuysBio/
│
├── index.html          # File giao diện chính
├── index.js            # Bun server
├── avatar.jpg         # Avatar
├── background.mp4     # Video background
├── album_default.jpg  # Cover nhạc mặc định
├── qr.png             # QR thanh toán
│
├── music/
│   ├── song1.mp3
│   ├── song2.mp3
│   └── ...
│
└── logo/
    ├── facebook.png
    ├── tiktok.png
    ├── roblox.png
    └── myprofile.png
```

---

## ⚙️ Requirements

Cài đặt:

* Bun runtime
  Download: https://bun.sh

Kiểm tra:

```bash
bun --version
```

---

## 🚀 Run Project

### 1. Clone repo

```bash
git clone https://github.com/yourusername/WuysBio.git
cd WuysBio
```

### 2. Chạy server

```bash
bun run index.js
```

hoặc

```bash
bun index.js
```

Server sẽ chạy tại:

```
http://localhost:10267
```

hoặc:

```
http://your-ip:10267
```

---

## 🎵 Thêm hoặc chỉnh sửa nhạc

Mở file:

```
index.html
```

Tìm phần:

```js
tracks: [
  { name: "Song name", file: "music/song1.mp3" },
]
```

Thêm bài hát:

```js
{ name: "My Song", file: "music/mysong.mp3" }
```

và đặt file mp3 vào thư mục `music/`

---

## 👤 Chỉnh sửa thông tin cá nhân

Mở:

```
index.html
```

Chỉnh sửa:

Avatar:

```html
<img id="avatar" src="avatar.jpg">
```

Tên:

```html
<h1>Welcome, world.</h1>
```

Bio:

```html
<h2>Hi~i I'm Wuys, This is my bio.</h2>
```

Social links:

```html
<a href="https://facebook.com/yourprofile">
```

---

## 🎥 Thay video background

Thay file:

```
background.mp4
```

hoặc chỉnh:

```html
<source src="background.mp4" type="video/mp4">
```

---

## 💳 Chỉnh QR Payment

Thay file:

```
qr.png
```

---

## 🌐 Deploy lên VPS

Upload toàn bộ file lên VPS

Run:

```bash
bun index.js
```

Mở port:

```
10267
```

Truy cập:

```
http://your-vps-ip:10267
```

---

## 🧠 Inspired by

guns.lol

---

## 📜 License

Free to use and modify.

---

## 👑 Author

Wuys

---

## ❤️ Notes

Server hỗ trợ:

* mp4 streaming
* mp3 streaming
* range requests
* fast static serving

Rất nhẹ và nhanh.
