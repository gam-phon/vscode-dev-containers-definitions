FROM golang:latest

RUN go get -v \
    # Base Go tools needed for VS code Go extension
    golang.org/x/tools/gopls \
    github.com/sqs/goreturns \
    github.com/rogpeppe/godef \
    github.com/mdempsky/gocode \
    github.com/godoctor/godoctor \
    github.com/stamblerre/gocode \
    github.com/ramya-rao-a/go-outline \
    github.com/acroca/go-symbols \
    # github.com/uudashr/gopkgs/cmd/gopkgs@latest \
    github.com/uudashr/gopkgs/cmd/gopkgs \
    golang.org/x/tools/cmd/guru \
    golang.org/x/tools/cmd/gorename \
    golang.org/x/lint/golint \
    github.com/go-delve/delve/cmd/dlv \
    # Extra tools integrating with VS code
    github.com/fatih/gomodifytags \
    github.com/haya14busa/goplay/cmd/goplay \
    github.com/josharian/impl \
    # github.com/tylerb/gotype-live \
    github.com/cweill/gotests/... \
    github.com/davidrjenni/reftools/cmd/fillstruct \
    # Terminal tools
    # github.com/vektra/mockery/... \
    2>&1 && \
    rm -rf /go/pkg /go/src/* /root/.cache/go-build
