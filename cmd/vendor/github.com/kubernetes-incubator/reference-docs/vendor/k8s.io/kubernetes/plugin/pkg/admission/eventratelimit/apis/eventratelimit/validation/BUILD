package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_library(
    name = "go_default_library",
    srcs = ["validation.go"],
    importpath = "k8s.io/kubernetes/plugin/pkg/admission/eventratelimit/apis/eventratelimit/validation",
    tags = ["automanaged"],
    deps = [
        "//vendor/k8s.io/apimachinery/pkg/util/validation/field:go_default_library",
        "//vendor/k8s.io/kubernetes/plugin/pkg/admission/eventratelimit/apis/eventratelimit:go_default_library",
    ],
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
)

go_test(
    name = "go_default_test",
    srcs = ["validation_test.go"],
    importpath = "k8s.io/kubernetes/plugin/pkg/admission/eventratelimit/apis/eventratelimit/validation",
    library = ":go_default_library",
    tags = ["automanaged"],
    deps = ["//vendor/k8s.io/kubernetes/plugin/pkg/admission/eventratelimit/apis/eventratelimit:go_default_library"],
)
