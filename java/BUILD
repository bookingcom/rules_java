load("@bazel_skylib//:bzl_library.bzl", "bzl_library")

package(default_visibility = ["//visibility:public"])

licenses(["notice"])

# TODO(aiuto): Find a way to strip this rule from the distribution tarball.
filegroup(
    name = "distribution",
    srcs = glob([
        "**",
    ]) + [
        "//java/constraints:srcs",
    ],
    visibility = [
        "@//distro:__pkg__",
    ],
)

bzl_library(
    name = "rules",
    srcs = ["defs.bzl"],
    visibility = ["//visibility:public"]
)
