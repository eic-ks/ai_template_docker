
FROM python:3.12-slim

# 基本ツール（AI・Kaggle開発向け）
RUN apt-get update && apt-get install -y \
    git \
    curl \
    wget \
    unzip \
    zip \
    tree \
    less \
    build-essential \
    && rm -rf /var/lib/apt/lists/*

# pipを最新化
RUN pip install --upgrade pip

# uv
RUN pip install --no-cache-dir uv

# 作業ディレクトリ
WORKDIR /workspace

# デフォルトはbash
CMD ["/bin/bash"]