load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "client.go",
        "dsn.go",
        "hub.go",
        "integrations.go",
        "interfaces.go",
        "scope.go",
        "sentry.go",
        "sourcereader.go",
        "stacktrace.go",
        "transport.go",
        "util.go",
    ],
    importmap = "k8s.io/kubernetes/vendor/github.com/getsentry/sentry-go",
    importpath = "github.com/getsentry/sentry-go",
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
