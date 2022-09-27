# Use local_repository if you're pointing to a local directory that already has
# a WORKSPACE file. You can also use bzlmod or http_repository to pull directly
# from official sources if you prefer.
local_repository(
    name = "bazel_skylib",
    path = "third_party/bazel-skylib/",
)

load("@bazel_skylib//:workspace.bzl", "bazel_skylib_workspace")
bazel_skylib_workspace()

# Use new_local_repository if you're pointing to a local directory that does
# *not* have a WORKSPACE/BUILD file. This essentially recreates the directory
# you point to with the path argument and sticks build_file and
# workspace_file_content in there for use inside the sandbox.
# This is typically used when you don't have control over the repository that
# you're importing (as is the case here) and thus can't add a BUILD or WORKSPACE
# file upstream.
new_local_repository(
    name = "cppfront",
    build_file = "third_party/cppfront-bzl-rules/BUILD.cppfront.bzl",
    path = "third_party/cppfront/",
    workspace_file_content = "",
)
