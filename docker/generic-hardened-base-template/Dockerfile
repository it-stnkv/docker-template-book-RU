FROM debian:stable-slim

ENV APP_HOME=/app

WORKDIR $APP_HOME

RUN apt-get update \
 && apt-get install -y --no-install-recommends ca-certificates curl \
 && rm -rf /var/lib/apt/lists/*

RUN useradd -m -s /bin/bash appuser

COPY . .

RUN chown -R appuser:appuser $APP_HOME

USER appuser

CMD ["./start.sh"]
