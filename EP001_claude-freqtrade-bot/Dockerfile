FROM freqtradeorg/freqtrade:latest

WORKDIR /freqtrade

# 只复制你的策略和配置到容器里
COPY . .

# 如果需要额外的 Python 包（可选）
# RUN if [ -f requirements.txt ]; then pip install -r requirements.txt; fi

# Freqtrade 的默认启动方式
CMD ["freqtrade"]
