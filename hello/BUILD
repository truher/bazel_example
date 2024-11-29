load("@nanobind_bazel//:build_defs.bzl", "nanobind_extension")

cc_library(
    name = "hello_lib",
    srcs = ["speaker.cpp"],
    hdrs = ["speaker.h"],
    visibility = ["//visibility:public"],
)

nanobind_extension(
    name = "hello",  # must be the same as the cpp file
    srcs = [
        "hello.cpp",
        "speaker.h",
    ],
    visibility = ["//visibility:public"],
    deps = [":hello_lib"],
)
