load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "ipsock_linux.go",
        "sctp.go",
        "sctp_linux.go",
        "sctp_unsupported.go",
    ],
    importmap = "k8s.io/kubernetes/vendor/github.com/ishidawataru/sctp",
    importpath = "github.com/ishidawataru/sctp",
    visibility = ["//visibility:public"],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [":package-srcs"],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
