FROM node:22-slim

LABEL maintainer="knight2010" \
      description="EP009 Jev 中高频交易测试台" \
      version="1.0"

WORKDIR /app

COPY . .

EXPOSE 8770

# 启动网页服务
# HOST=0.0.0.0 让服务监听所有网卡
# ALLOW_HOST 通过环境变量指定允许的外部 Host（防 DNS 重绑定），格式：hostname 或 hostname:port
CMD ["sh", "-c", "node jev-hft-bench/server.mjs --host ${HOST:-0.0.0.0} $([ -n \"$ALLOW_HOST\" ] && echo \"--allow-host $ALLOW_HOST\" || echo '')"]
