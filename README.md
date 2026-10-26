# Tính Lợi Nhuận Shopee

Công cụ web một trang giúp tính nhanh lợi nhuận từng sản phẩm khi bán trên Shopee, so sánh cùng lúc trên 6 gian hàng (Nhà Sách, CN1, CN2, Tường Vip, Tranh Vip, Tường Vip New) theo 5 ngành hàng (Sách, Tranh, Lịch, Decal, Trà).

## Tính năng

- Nhập sản phẩm thủ công hoặc import từ file Excel (.xlsx, .xls), có file mẫu tải về.
- Tự tính lợi nhuận và tỷ suất lợi nhuận (%) theo từng gian hàng.
- Tuỳ chỉnh các khoản phí sàn (phí cố định, voucher, phí xử lý giao dịch, phí dịch vụ, quảng cáo, aff, phí hạ tầng…) cho từng gian và ngành.
- Xuất báo cáo lợi nhuận ra file Excel.
- Dữ liệu sản phẩm và cấu hình được lưu ngay trên trình duyệt (localStorage).

## Cách dùng

1. Mở file `index.html` bằng trình duyệt (cần kết nối mạng để tải thư viện đọc/ghi Excel).
2. Vào tab **Cấu hình chi phí**, kiểm tra/điều chỉnh % phí cho từng gian hàng rồi bấm **Lưu cấu hình**.
3. Quay lại tab **Tính lợi nhuận**:
   - Bấm **Thêm dòng** để nhập tay, hoặc kéo thả file Excel có các cột: Tên sản phẩm, Phân loại, Ngành hàng, Giá vốn, Giá bán.
   - Xem lợi nhuận từng gian ngay trên bảng và phần **Báo cáo tổng kết** bên dưới.
4. Bấm **Xuất Excel** để tải báo cáo về máy.

## Công thức

```
Lợi nhuận = Giá bán − Giá vốn − Phí hạ tầng − Giá bán × (Tổng % các khoản phí)
```
