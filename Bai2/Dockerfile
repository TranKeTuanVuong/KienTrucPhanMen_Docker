# Sử dụng Python 3.9 làm base image
FROM python:3.9

# Thiết lập thư mục làm việc trong container
WORKDIR /app

# Sao chép các file cần thiết vào container
COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt

# Sao chép toàn bộ code vào container
COPY . .

# Mở cổng 5000
EXPOSE 5000

# Chạy ứng dụng
CMD ["python", "app.py"]
