# Description:
#   Contains deprecated functions that we aren't quite ready to remove entirely

load("//tensorflow:tensorflow.bzl", "py_test")

package(
    default_visibility = ["//tensorflow:__subpackages__"],
    licenses = ["notice"],  # Apache 2.0
)

exports_files(["LICENSE"])

py_library(
    name = "deprecated_py",
    srcs = ["__init__.py"],
    srcs_version = "PY2AND3",
    deps = [
        "//tensorflow/python:logging_ops",
        "//tensorflow/python:util",
    ],
)

py_test(
    name = "summaries_test",
    srcs = ["summaries_test.py"],
    python_version = "PY2",
    srcs_version = "PY2AND3",
    deps = [
        "//tensorflow/python:array_ops",
        "//tensorflow/python:client_testlib",
        "//tensorflow/python:framework_for_generated_wrappers",
        "//tensorflow/python:logging_ops",
    ],
)
