# Sử dụng Node.js LTS (18) trên Alpine
FROM node:18-alpine

# Tạo thư mục làm việc trong container
WORKDIR /app

# Copy package.json và package-lock.json trước
COPY package*.json ./

# Cài đặt dependencies
RUN npm install --production

# Copy toàn bộ code vào container
COPY . .

# Expose port (giống với cổng backend chạy trong code, ví dụ 5000)
EXPOSE 5000

# Lệnh khởi chạy
CMD ["npm", "start"]
