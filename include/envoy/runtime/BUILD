licenses(["notice"])  # Apache 2

load(
    "//bazel:envoy_build_system.bzl",
    "envoy_cc_library",
    "envoy_package",
)

envoy_package()

envoy_cc_library(
    name = "runtime_interface",
    hdrs = ["runtime.h"],
    external_deps = ["abseil_optional"],
    deps = [
        "//source/common/common:assert_lib",
        "//source/common/singleton:threadsafe_singleton",
        "@envoy_api//envoy/type/v3alpha:pkg_cc_proto",
    ],
)
