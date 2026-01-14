# Laboratory Management System


## Công nghệ sử dụng

### Frontend
- React 19.2.0
- TypeScript 5.8.3
- Vite 7.1.7
- Tailwind CSS 4.1.14
- React Router DOM 7.9.1
- Axios 1.12.2
- Formik 2.4.6
- React Toastify 11.0.5

### Backend
- Node.js 18.0.0
- Express.js 5.1.0
- MongoDB (Mongoose 8.18.2)
- JWT Authentication (jsonwebtoken 9.0.2)
- Bcrypt 6.0.0
- Google Auth Library 10.4.1
- Swagger Documentation (swagger-ui-express 5.0.1, swagger-jsdoc 6.2.8)
- Nodemailer 7.0.6
- Axios 1.12.2
- CORS 2.8.5
- Dotenv 17.2.2
- Joi 18.0.1
- UUID 9.0.1
- Nodemon 3.1.10

## Cài đặt và chạy

### 1. Clone repository
```bash
git clone <repository-url>
cd laboratory-management
```

### 2. Cài đặt dependencies

#### Backend
```bash
cd BE
npm install
```

#### Frontend
```bash
cd FE
npm install
```

### 3. Chạy dự án

#### Chạy Backend (Terminal 1)
```bash
cd BE
npm start
# hoặc
npm run dev
```

#### Chạy Frontend (Terminal 2)
```bash
cd FE
npm run dev
```

### 4. Truy cập ứng dụng
## Cấu trúc dự án

```
laboratory-management/
├── BE/                     # Backend API
│   ├── app.js             # Entry point
│   ├── config/            # Database & mail config
│   ├── controllers/       # API controllers
│   ├── models/            # Database models
│   ├── routes/            # API routes
│   ├── middlewares/       # Custom middlewares
│   ├── validations/       # Input validations
│   ├── helpers/           # Utility functions
│   └── docs/              # Swagger documentation
├── FE/                     # Frontend React App
│   ├── src/
│   │   ├── components/    # Reusable components
│   │   ├── contexts/      # React contexts
│   │   ├── router/        # Router configuration
│   │   ├── source/
│   │   │   ├── page/      # Page components
│   │   │   │   ├── Admin/     # Admin pages
│   │   │   │   ├── Doctor/    # Doctor pages
│   │   │   │   ├── Nurse/     # Nurse pages
│   │   │   │   ├── Patient/   # Patient pages
│   │   │   │   └── Home/      # Home page
│   │   │   └── Axios/     # API configuration
│   │   └── utils/         # Utility functions
│   ├── public/            # Static assets
│   └── dist/              # Build output
└── README.md              # This file
```

## Tính năng chính

### 🔐 Xác thực & Phân quyền
- Đăng nhập/Đăng ký với JWT
- Phân quyền theo vai trò (Admin, Doctor, Nurse, Patient)
- Bảo mật API với middleware

### 👥 Quản lý người dùng
- Quản lý tài khoản người dùng
- Cập nhật thông tin cá nhân
- Lịch sử hoạt động

### 🧪 Quản lý phòng thí nghiệm
- **Thiết bị**: Theo dõi và quản lý thiết bị
- **Hóa chất**: Quản lý tồn kho và sử dụng
- **Đơn xét nghiệm**: Tạo và theo dõi đơn xét nghiệm
- **Kết quả**: Nhập và xem kết quả xét nghiệm

### 📊 Báo cáo & Thống kê
- Dashboard với biểu đồ thống kê
- Báo cáo xuất PDF
- Lịch sử hoạt động chi tiết

### 🔔 Thông báo
- Hệ thống thông báo real-time
- Email notifications
- In-app notifications

## API Endpoints

### Base URLs
- **Local Development**: `http://localhost:5000`
- **Production**: `https://deloy-project.vercel.app/`

### Authentication
- `POST /api/auth/login` - Đăng nhập
- `POST /api/auth/register` - Đăng ký
- `POST /api/auth/forgot-password` - Quên mật khẩu

### Test Results
- `GET /api/test-results` - Lấy danh sách kết quả
- `GET /api/test-results/:id` - Lấy chi tiết kết quả
- `POST /api/test-results` - Tạo kết quả mới
- `PUT /api/test-results/:id` - Cập nhật kết quả

### Instruments
- `GET /api/instruments` - Lấy danh sách thiết bị
- `POST /api/instruments` - Thêm thiết bị mới

### Frontend

#### Local Development
```bash
cd FE
npm run dev
# Development server
```

React + Vite



#### Local Development
```bash
cd BE
npm start
# Production mode
```

## Môi trường phát triển

### Yêu cầu hệ thống
- Node.js >= 16.0.0
- npm >= 8.0.0
- MongoDB >= 4.0




