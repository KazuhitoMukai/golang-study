FROM golang:1.19.1-alpine
# アップデートとgitのインストール
RUN apk update && \
    apk add bash git make && \
    apk add --upgrade grep

# パッケージのインポート
# linter staticcheck導入
RUN go install honnef.co/go/tools/cmd/staticcheck@latest

# mysql導入
WORKDIR /go/src/app
RUN go mod init hello-go
RUN go get -u github.com/go-sql-driver/mysql@v1.7.0