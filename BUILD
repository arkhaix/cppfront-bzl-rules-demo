load("//:third_party/cppfront-bzl-rules/cppfront_rules.bzl", "cpp2_library")

cpp2_library(
    name = "hello_world_cpp2",
    srcs = ["foo.cpp2"],
)

cc_binary(
    name = "hello_world",
    deps = [":hello_world_cpp2"],
)
