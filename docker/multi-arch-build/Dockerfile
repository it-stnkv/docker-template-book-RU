FROM --platform=$BUILDPLATFORM golang:1.22 AS builder

ARG TARGETOS
ARG TARGETARCH

WORKDIR /app
COPY . .

RUN GOOS=$TARGETOS GOARCH=$TARGETARCH go build -o app

FROM alpine:3.19

COPY --from=builder /app/app .

CMD ["./app"]
