# cppfront-bzl-rules-demo
Demo repository for cppfront-bzl-rules

# Instructions
Make sure that you build with `-std=c++20`.

```sh
$ bazel build --copt="-std=c++20" :hello_world
```

# Inspect generated .cpp file
Note that the exact path on your computer may differ

```sh
$ bazel build --copt="-std=c++20" :hello_world_cpp2
$ less bazel-out/k8-fastbuild/bin/foo.cpp
```
