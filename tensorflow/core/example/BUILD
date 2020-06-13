package(default_visibility = ["//visibility:public"])

load("@rules_proto//proto:defs.bzl", "proto_library")
load("@rules_cc//cc:defs.bzl", "cc_binary", "cc_proto_library")
load("@com_github_grpc_grpc//bazel:python_rules.bzl", "py_proto_library")

proto_library(
    name = "feature_proto",
    srcs = ["feature.proto"],
)

cc_proto_library(
    name = "feature_cc_proto",
    deps = [":feature_proto"],
)

py_proto_library(
    name = "feature_py_proto",
    deps = [":feature_proto"]
)
