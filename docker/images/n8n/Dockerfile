# Dùng image build sẵn của n8n (siêu nhanh)
FROM n8nio/n8n

# Làm việc trong thư mục mặc định
WORKDIR /home/node

# Copy .env nếu cần (hoặc set qua Render UI)
# COPY .env /home/node/.env

# (Tùy chọn) Nếu có script entrypoint tùy biến
# COPY docker-entrypoint.sh /docker-entrypoint.sh
# ENTRYPOINT ["tini", "--", "/docker-entrypoint.sh"]

# Sửa quyền thư mục nếu cần
RUN mkdir -p /home/node/.n8n && chown node:node /home/node/.n8n

# Chạy bằng user node
USER node
