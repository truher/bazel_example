# load("@rules_python//python:defs.bzl", "py_binary")

py_binary(
    name = "hello_client",
    srcs = ["client.py"],
    data = ["//hello"],
    imports = ["../hello"],
    main = "client.py",
    visibility = ["//visibility:public"],
)
