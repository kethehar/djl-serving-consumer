# cd djl-serving
# docker build -t mosazhaw/djl-serving:latest .
# docker push mosazhaw/djl-serving:latest

FROM deepjavalibrary/djl-serving:0.36.0

ENV SERVING_RESERVED_MEMORY_MB=64 \
    SERVING_REQUIRED_MEMORY_MB=64 \
    SERVING_MIN_WORKERS=1 \
    SERVING_MAX_WORKERS=1 \
    JAVA_OPTS="-Xms64m -Xmx256m"

# Copy Model
COPY model /opt/ml/model