# Sơ đồ thư mục dự án
```
📁 BTL-ATBM/
│
├── app.py                   # Điểm khởi động Flask app
├── .env                     # Biến môi trường (DB, SECRET_KEY, ...)
├── requirements.txt         # Các thư viện cần cài
│
├── models.py                # Định nghĩa bảng User & LoginLog
├── utils.py                 # Xử lý SHA, salt, Triple DES
├── auth.py                  # Xử lý logic: đăng ký, đăng nhập, đổi mật khẩu
│
├── templates/               # Giao diện HTML
│   ├── layout.html
│   ├── index.html
│   ├── register.html
│   ├── login.html
│   ├── change_password.html
│   └── admin.html
│
└── static/                  # CSS, JS, ảnh (nếu có)
```
# Nội dung file .env
```
DB_SERVER=localhost
DB_NAME=FlaskAuth
DB_DRIVER=ODBC Driver 17 for SQL Server
USE_WINDOWS_AUTH=True
SECRET_KEY=your_secret_key_here
```
# Cách chạy
## Lệnh cấp phép tạm thời
```
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope Process
```
## Tạo/Kích hoạt môi trường ảo
```
python -m venv venv
.\venv\Scripts\activate
```
## Tải thư viện
```
pip install -r requirements.txt
```
## Chạy dự án
```
python app.py
```
