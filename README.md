# 🎬 Hệ Thống Quản Lý Rạp Chiếu Phim

---

## Mô tả hệ thống:
- Quản lý thông tin phim, rạp chiếu, phòng chiếu và ghế ngồi
- Quản lý lịch suất chiếu
- Đặt vé và quản lý khách hàng
- Phân công nhân viên phụ trách suất chiếu

---

## Các bảng trong database

| Bảng | Mô tả |
|---|---|
| `PHIM` | Thông tin bộ phim |
| `RAP_CHIEU` | Thông tin rạp chiếu |
| `PHONG_CHIEU` | Các phòng chiếu trong rạp |
| `GHE` | Ghế ngồi trong từng phòng |
| `SUAT_CHIEU` | Lịch chiếu phim |
| `VE` | Vé đã được đặt |
| `KHACH_HANG` | Thông tin khách hàng |
| `NHAN_VIEN` | Thông tin nhân viên |
| `PHAN_CONG` | Phân công nhân viên – suất chiếu (N-N) |

---

## ⚙️ Hướng dẫn chạy

### Yêu cầu
- PostgreSQL 13 trở lên

### Các bước thực hiện

**Bước 1:** Tạo database mới
```sql
CREATE DATABASE rap_chieu_phim;
```

**Bước 2:** Chạy file SQL

```bash
psql -U postgres -d rap_chieu_phim -f rap_chieu_phim.sql
```

Hoặc mở file `rap_chieu_phim.sql` trong **pgAdmin** → Query Tool → Execute.

---
