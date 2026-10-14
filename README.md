# Thực hành tạo dự án mới trên GitHub

## Mục tiêu

Tạo một repository Git cục bộ, kết nối với repository trên GitHub, rồi đưa `README.md` lên GitHub.

## Ý nghĩa các lệnh Git

| Lệnh | Ý nghĩa |
| --- | --- |
| `git init -b main` | Khởi tạo repository Git cục bộ mới với nhánh chính tên `main`. |
| `git remote add origin https://github.com/USERNAME/REPOSITORY.git` | Thêm địa chỉ repository GitHub từ xa và đặt bí danh cho địa chỉ đó là `origin`. Thay URL mẫu bằng URL repository vừa tạo. |
| `git add README.md` | Đưa `README.md` vào staging area, tức chọn tệp sẽ được lưu trong commit tiếp theo. |
| `git commit -m "Add README.md file"` | Tạo một commit lưu lại các thay đổi đã stage. Tùy chọn `-m` ghi lời mô tả ngắn cho commit. |
| `git push -u origin main` | Đẩy các commit trên nhánh `main` lên remote tên `origin`. Tùy chọn `-u` thiết lập nhánh upstream để các lần push sau thuận tiện hơn. |

## Các bước đồng bộ

1. Tạo repository mới trên GitHub. Nếu muốn dùng các lệnh push bên dưới, không khởi tạo sẵn README trên GitHub.
2. Mở Terminal tại thư mục dự án này.
3. Thêm remote bằng URL repository của bạn:

   ```bash
   git remote add origin https://github.com/USERNAME/REPOSITORY.git
   ```

4. Đưa README vào staging area và tạo commit:

   ```bash
   git add README.md
   git commit -m "Add README.md file"
   ```

5. Đẩy nhánh chính lên GitHub:

   ```bash
   git push -u origin main
   ```

Sau khi push thành công, mở trang repository GitHub và kiểm tra README đã xuất hiện. Thay `USERNAME/REPOSITORY` bằng tên tài khoản và repository thật trước khi chạy lệnh.
