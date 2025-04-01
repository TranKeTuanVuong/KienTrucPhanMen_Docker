# Sử dụng Node.js base image
FROM node:16

# Tạo thư mục làm việc trong container
WORKDIR /usr/src/app

# Sao chép package.json và cài đặt các dependencies
COPY package*.json ./
RUN npm install

# Sao chép toàn bộ mã nguồn vào container
COPY . .

# Mở cổng 3000
EXPOSE 3000

# Chạy ứng dụng Node.js
CMD ["npm", "start"]
