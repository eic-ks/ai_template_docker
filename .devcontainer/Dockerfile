FROM python:3.12-slim

# 基本ツール（最低限の開発環境）
RUN apt-get update && apt-get install -y \
    git \
    curl \
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