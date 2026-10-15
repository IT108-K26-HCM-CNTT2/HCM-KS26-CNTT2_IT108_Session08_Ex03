# Tài liệu Hướng dẫn Cài đặt và Sử dụng VS Code cho Lớp học

## 1. Báo cáo phân tích (I/O)

- **Input (Văn bản thô):** Nội dung tài liệu dạng văn bản thuần túy được viết bằng Markdown, trong đó sử dụng các ký tự thoát (`\`) để hiển thị nguyên bản các ký tự đặc biệt như `\*` hay `\#` mà không kích hoạt tính năng định dạng, cùng với cấu trúc code block, table và task list.
- **Output (Giao diện hiển thị trên StackEdit):** 
  - Các ký tự đặc biệt được hiển thị chính xác như ký tự văn bản thông thường.
  - Các đoạn code Python được tô màu cú pháp (Syntax Highlighting) sinh động.
  - Bảng so sánh giữa StackEdit và VS Code được sắp xếp ngay ngắn, dễ đọc.
  - Danh sách công việc (Task List) hiển thị dưới dạng các hộp kiểm (checkbox) có thể tương tác.

---

## 2. Nội dung hướng dẫn chi tiết

### I. Giới thiệu chung
Chào mừng các bạn đến với buổi thực hành lập trình. Trong quá trình học, chúng ta sẽ làm quen với việc sử dụng biến cơ bản như `variable_name` và công cụ soạn thảo mã nguồn chuyên nghiệp `VS Code`.

\# Lưu ý quan trọng: Không được bỏ qua bước cấu hình môi trường dưới đây nếu không muốn gặp lỗi khi chạy code \*Python\*.

---

### II. Kiểm tra môi trường với Python
Dưới đây là đoạn mã Python mẫu dùng để kiểm tra cấu hình hệ thống của bạn:

```python
def check_environment(student_name: str) -> None:
    """Hàm kiểm tra môi trường học tập của học viên."""
    version_info = "Python 3.10+"
    print(f"Xin chào {student_name}! Môi trường hiện tại: {version_info}")

if __name__ == "__main__":
    check_environment("Học viên lớp mới")
```

---

### III. So sánh StackEdit và VS Code

| Tiêu chí | StackEdit | VS Code |
| :--- | :--- | :--- |
| **Mục đích chính** | Soạn thảo tài liệu Markdown trực tuyến | Môi trường phát triển tích hợp (IDE) chuyên nghiệp |
| **Hỗ trợ Code** | Hỗ trợ xem trước Markdown, không chạy được code phức tạp | Hỗ trợ chạy, gỡ lỗi (debug) và quản lý dự án lớn |
| **Tính lưu trữ** | Đồng bộ đám mây (Cloud), trình duyệt web | Lưu trữ cục bộ trên máy tính (Local) |

---

### IV. Task List kiểm tra tiến độ cài đặt
Hãy đánh dấu hoàn thành các bước dưới đây để đảm bảo máy tính của bạn đã sẵn sàng:

- [x] Tải và cài đặt phần mềm VS Code từ trang chủ.
- [ ] Cài đặt Extension `Python` và `Pylance` trong VS Code.
- [ ] Cấu hình Terminal mặc định trỏ tới `PowerShell` hoặc `Bash`.
- [ ] Tạo file `main.py` đầu tiên và chạy thử nghiệm thành công.