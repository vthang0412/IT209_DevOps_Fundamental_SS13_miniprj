# Campus Hub Base — Docker

## 1. Thông tin sinh viên
- **Họ tên:** Đặng Văn Thắng

## 2. Lệnh chạy hệ thống

Chạy tại thư mục gốc repository:

```powershell
docker compose up -d --build
```

Kiểm tra trạng thái các service:

```powershell
docker compose ps
```

Dừng hệ thống:

```powershell
docker compose down
```

## 3. Cổng và URL kiểm tra backend

- **Backend:** http://localhost:8080
- **Health endpoint:** http://localhost:8080/actuator/health
- **MySQL:** localhost:3307

Kiểm tra trạng thái backend bằng PowerShell:

```powershell
curl.exe -i http://localhost:8080/actuator/health
```

Kết quả mong đợi: HTTP 200 và trạng thái `"UP"`.