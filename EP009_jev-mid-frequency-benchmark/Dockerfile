FROM node:22-slim

LABEL maintainer="knight2010" \
      description="EP009 Jev 中高频交易测试台" \
      version="1.0"

WORKDIR /app

COPY . .

# Node.js 22 无需额外依赖（零依赖设计）
EXPOSE 8770

# 启动网页服务
CMD ["node", "jev-hft-bench/server.mjs"]
