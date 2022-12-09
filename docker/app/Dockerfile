FROM golang:1.19.1-alpine
# アップデートとgitのインストール
RUN apk update
# パッケージのインポート
# linter staticcheck導入
RUN go install honnef.co/go/tools/cmd/staticcheck@latest
# mysql導入
RUN go install github.com/go-sql-driver/mysql@latest