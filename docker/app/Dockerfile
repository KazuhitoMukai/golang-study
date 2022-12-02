FROM golang:1.19.1-alpine
# アップデートとgitのインストール
RUN apk update
# パッケージのインポート

RUN go get github.com/go-sql-driver/mysql
# linter staticcheck導入
RUN go install honnef.co/go/tools/cmd/staticcheck@latest