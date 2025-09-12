# DuAn12T9 - Sơ đồ Kiến trúc Micro-Frontend & BFF

## 📋 Mô tả dự án

Dự án này chứa các sơ đồ kiến trúc Micro-Frontend và Backend for Frontend (BFF) được thiết kế bằng HTML/CSS và Mermaid.js.

## 🏗️ Kiến trúc hệ thống

### 🖥️ Frontend Layer
- **Shell Applications**: User & Admin Shell Apps
- **Micro-Frontend Modules**: Product, Cart, News (User & Admin versions)

### 🔗 BFF Layer (Backend for Frontend)
- **User BFF**: Xử lý requests từ user applications
- **Admin BFF**: Xử lý requests từ admin applications

### ⚡ Backend Microservices
- **Configuration Services**: Shell Config Service
- **Core Services**: Admin Service, Agent Policy Service, Agent Management Service
- **Business Services**: Football Service ⚽, User Service, Payment Service
- **Extended Services**: Chatbot Service, Design Calculation Service, Football Analytics Service ⚽
- **New Services**: News Service, Cart Service, Product Service

### 🗄️ Database & Infrastructure
- **Databases**: Tương ứng với từng service
- **Infrastructure**: Message Broker, Cache

## 📁 Cấu trúc file

```
├── README.md                           # File mô tả dự án
├── microservice-fixed.html            # Sơ đồ HTML đã sửa lỗi (KHUYẾN NGHỊ)
├── microservice-black-text.html       # Sơ đồ HTML với text đen đậm
├── microservice-clean.html            # Sơ đồ HTML phiên bản đơn giản
├── microservice-football-analytics.mmd # File Mermaid gốc
├── microservice-football-analytics.svg # File SVG được generate
├── microservice-football-final.svg    # File SVG phiên bản cuối
├── puppeteer-config.json             # Cấu hình Puppeteer cho Mermaid CLI
└── package.json                       # Dependencies cho Mermaid CLI
```

## 🚀 Cách sử dụng

### 1. Xem sơ đồ trực tiếp
Mở file `microservice-fixed.html` trong trình duyệt để xem sơ đồ interactive.

### 2. Tính năng có sẵn
- ✅ **Zoom In/Out**: Sử dụng nút hoặc phím +/-
- ✅ **Pan**: Kéo thả bằng chuột trái
- ✅ **Reset Zoom**: Phím 0 hoặc nút Reset
- ✅ **Fit to Screen**: Phím F hoặc nút Fit Screen
- ✅ **Text đen đậm**: Tất cả text hiển thị rõ ràng

### 3. Generate SVG từ Mermaid
```bash
# Cài đặt dependencies
npm install

# Generate SVG
npx @mermaid-js/mermaid-cli -i microservice-football-analytics.mmd -o output.svg -p puppeteer-config.json
```

## 🎯 Đặc điểm nổi bật

- **Không có vùng đen che phủ**: Đã khắc phục hoàn toàn vấn đề render
- **Interactive**: Có thể zoom, pan, và điều khiển bằng keyboard
- **Responsive**: Tự động điều chỉnh theo kích thước màn hình
- **Clean Design**: Giao diện sạch sẽ, dễ đọc
- **Multiple Formats**: Hỗ trợ HTML, SVG, và Mermaid

## 🔧 Công nghệ sử dụng

- **HTML5/CSS3**: Giao diện và styling
- **Mermaid.js**: Tạo sơ đồ flowchart
- **JavaScript**: Tương tác và điều khiển
- **Node.js**: Mermaid CLI để generate SVG
- **Puppeteer**: Headless browser cho rendering

## 📝 Lịch sử phiên bản

- **v1.0**: Sơ đồ cơ bản với subgraph phức tạp
- **v2.0**: Thêm Football Service thay thế Contract Service
- **v3.0**: Thêm Football Analytics Service thay thế Inventory Management
- **v4.0**: Sửa lỗi màu đen che phủ, tối ưu hiển thị

## 👨‍💻 Tác giả

**khpt1976-cloud**
- GitHub: [@khpt1976-cloud](https://github.com/khpt1976-cloud)

## 📄 License

Dự án này được phát hành dưới MIT License.

---

⚽ **Đặc biệt**: Hệ thống tập trung vào các dịch vụ bóng đá với Football Service và Football Analytics Service!
