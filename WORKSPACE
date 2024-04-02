load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")
load("@bazel_tools//tools/cpp:cc_configure.bzl", "cc_configure")
load("@bazel_tools//tools/build_defs/repo:git.bzl", "git_repository")

cc_configure()

git_repository(
    name = "parlaylib",
    remote = "https://github.com/ParAlg/parlaylib.git",
    commit = "6b4a4cdbfeb3c481608a42db0230eb6ebb87bf8d",
    strip_prefix = "include/",
)

http_archive(
    name = "googletest",
    sha256 = "b4870bf121ff7795ba20d20bcdd8627b8e088f2d1dab299a031c1034eddc93d5",
    strip_prefix = "googletest-release-1.11.0",
    urls = ["https://github.com/google/googletest/archive/release-1.11.0.tar.gz"],
)
