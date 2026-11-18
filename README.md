# Quản lý quán ăn

Ứng dụng quản lý quán ăn gồm backend NestJS và frontend React/Vite.

## Cấu trúc

- `be-smart-menu/`: API backend.
- `fe-smart-menu/`: giao diện frontend.

## Chạy trên máy cá nhân

Yêu cầu Node.js và npm.

1. Tạo file cấu hình từ mẫu:
   - Backend: sao chép `be-smart-menu/.env.example` thành `be-smart-menu/.env`.
   - Frontend: sao chép `fe-smart-menu/.env.example` thành `fe-smart-menu/.env.development`.
2. Điền cấu hình phù hợp với môi trường của bạn. Backend cần MongoDB; Redis và các dịch vụ Google, thanh toán, email, SMS cần thông tin tương ứng nếu sử dụng.
3. Cài dependencies và chạy backend:

   ```powershell
   cd be-smart-menu
   npm ci
   npm run start:dev
   ```

4. Mở terminal khác, cài dependencies và chạy frontend:

   ```powershell
   cd fe-smart-menu
   npm ci
   npm run dev
   ```

Không commit file `.env` hoặc thông tin bí mật. Chỉ các file `.env.example` với giá trị mẫu được đưa lên Git.

## Build

- Backend: chạy `npm run build` trong `be-smart-menu/`.
- Frontend: chạy `npm run build` trong `fe-smart-menu/`.
