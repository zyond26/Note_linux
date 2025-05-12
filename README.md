# Note tmux 

# 🧠 Ghi Chú Lệnh Cơ Bản TMUX

`tmux` là một công cụ mạnh để quản lý nhiều phiên terminal trong cùng một cửa sổ. Dưới đây là các lệnh và tổ hợp phím cơ bản cần ghi nhớ.

---

## 🔰 Khởi động và Quản lý Phiên (`Session`)

| Lệnh | Chức năng |
|------|-----------|
| `tmux` | Bắt đầu phiên tmux mới |
| `tmux new -s <ten>` | Tạo phiên mới với tên |
| `tmux ls` | Liệt kê các phiên đang chạy |
| `tmux attach -t <ten>` | Gắn vào phiên tmux có tên |
| `tmux kill-session -t <ten>` | Đóng phiên tmux |

---

## 🧩 Tổ Hợp Phím Điều Khiển (Prefix: `Ctrl + b`)

> Sau khi nhấn `Ctrl + b`, tiếp tục nhấn phím bên phải:

| Phím | Chức năng |
|------|-----------|
| `c` | Tạo cửa sổ mới |
| `n` | Chuyển tới cửa sổ tiếp theo |
| `p` | Quay lại cửa sổ trước |
| `,` | Đổi tên cửa sổ |
| `w` | Danh sách các cửa sổ |
| `&` | Đóng cửa sổ hiện tại |
| `d` | Tách khỏi tmux (detach) |
| `:` | Mở command-line của tmux |
| `[` | Vào chế độ xem lại đầu ra (scroll mode) |

---

## 🪟 Quản Lý Cửa Sổ (Window)

| Phím | Chức năng |
|------|-----------|
| `0` đến `9` | Chuyển tới cửa sổ tương ứng |
| `f` | Tìm cửa sổ theo tên |

---

## 🧱 Quản Lý Bảng (Pane)

| Phím | Chức năng |
|------|-----------|
| `"` | Chia ngang màn hình |
| `%` | Chia dọc màn hình |
| `o` | Di chuyển giữa các pane |
| `x` | Đóng pane hiện tại |
| `q` | Hiện số thứ tự các pane |

---

## 🛠 Lệnh Hữu Ích Khác

| Lệnh | Mô tả |
|------|-------|
| `tmux rename-session -t old_name new_name` | Đổi tên phiên |
| `tmux kill-server` | Tắt toàn bộ phiên tmux |

---

## 📌 Mẹo Sử Dụng

- Dùng `Ctrl + b`, sau đó nhấn `[` để vào chế độ cuộn, dùng phím `↑↓` để xem lại đầu ra cũ.
- Dùng `tmux` trong các phiên SSH để giữ trạng thái làm việc khi bị ngắt kết nối.
- Ghi nhớ prefix `Ctrl + b` là chìa khóa để dùng được tất cả chức năng của tmux.

---

## ✅ Nên Học và Thực Hành

- [ ] Tạo/đóng phiên tmux  
- [ ] Tạo/di chuyển cửa sổ và pane  
- [ ] Chia dọc/ngang và di chuyển giữa các pane  
- [ ] Tách và gắn lại vào phiên đang chạy  
- [ ] Cuộn lại log trong terminal bằng `[`  

---

> Ghi chú này dành cho các bạn mới học Linux/Pentest cần quản lý nhiều cửa sổ cùng lúc hiệu quả hơn với `tmux`.
