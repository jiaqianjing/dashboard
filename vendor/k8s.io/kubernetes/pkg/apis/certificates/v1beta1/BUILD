package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = [
        "conversion.go",
        "defaults.go",
        "doc.go",
        "generated.pb.go",
        "helpers.go",
        "register.go",
        "types.generated.go",
        "types.go",
        "types_swagger_doc_generated.go",
        "zz_generated.conversion.go",
        "zz_generated.deepcopy.go",
        "zz_generated.defaults.go",
    ],
    tags = ["automanaged"],
    deps = [
        "//pkg/api:go_default_library",
        "//pkg/apis/certificates:go_default_library",
        "//vendor:github.com/gogo/protobuf/proto",
        "//vendor:github.com/ugorji/go/codec",
        "//vendor:k8s.io/apimachinery/pkg/apis/meta/v1",
        "//vendor:k8s.io/apimachinery/pkg/conversion",
        "//vendor:k8s.io/apimachinery/pkg/runtime",
        "//vendor:k8s.io/apimachinery/pkg/runtime/schema",
        "//vendor:k8s.io/apimachinery/pkg/types",
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
