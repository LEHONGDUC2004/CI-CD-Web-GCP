
# CI-CD-Web-GCP

Dự án này là một ví dụ về triển khai CI/CD cho một ứng dụng web sử dụng Google Cloud Platform (GCP). Ứng dụng sử dụng Python (backend), HTML và CSS (frontend), và có hỗ trợ Docker để dễ dàng triển khai.

## Nội dung chính

- **Frontend:** HTML, CSS
- **Backend:** Python
- **Container hóa:** Docker
- **CI/CD:** Tích hợp tự động kiểm thử, build và deploy lên môi trường GCP

## Cấu trúc thư mục

```text
├── src/              # Mã nguồn ứng dụng web (Python, HTML, CSS)
├── Dockerfile        # Định nghĩa container
├── .github/workflows # Các workflow CI/CD với GitHub Actions
└── README.md         # Tài liệu dự án
```

## Yêu cầu

- Python 3.x
- Docker (nếu muốn chạy bằng container)
- Tài khoản GCP, đã thiết lập project và quyền truy cập
- GitHub Actions (CI/CD)

## Hướng dẫn sử dụng

### 1. Cài đặt các phụ thuộc

```bash
pip install -r requirements.txt
```

### 2. Chạy ứng dụng local

```bash
python src/app.py
```

### 3. Build Docker image

```bash
docker build -t web-app-gcp .
```

### 4. Đẩy lên Google Cloud (ví dụ với App Engine hoặc Cloud Run)

Xem hướng dẫn chi tiết trong các workflow CI/CD mẫu trong `.github/workflows`.

## CI/CD

- **Kiểm thử tự động:** Tự động chạy test khi có thay đổi mã nguồn.
- **Build & Deploy:** Tự động build Docker image và deploy lên GCP khi có merge vào nhánh chính.

## Đóng góp

Mọi đóng góp đều được chào đón! Hãy tạo pull request hoặc issue nếu bạn có ý tưởng hoặc phát hiện lỗi.

## License

MIT

---

> Dự án này dành cho học tập và demo CI/CD với GCP.  
