cc_library(
    name = "main",
    srcs = glob(
        ["googletest-release-1.8.0/googletest/src/*.cc",
         "googletest-release-1.8.0/googletest/src/*.h"],
        exclude = ["googletest-release-1.8.0/googletest/src/gtest-all.cc"]
    ),
    hdrs = glob([
        "googletest-release-1.8.0/googletest/include/**/*.h",
        "googletest-release-1.8.0/googletest/**/*.h"]),
    copts = ["-Iexternal/gtest/googletest-release-1.8.0/googletest/include",
             "-Iexternal/gtest/googletest-release-1.8.0/googletest"],
    linkopts = ["-pthread"],
    visibility = ["//visibility:public"],
)

cc_library(
    name = "local_main",
    srcs = glob(
        ["gtest/src/*.cc",
         "gtest/src/*.h"],
        exclude = ["gtest/src/gtest-all.cc"]
    ),
    hdrs = glob([
        "gtest/include/**/*.h",
        "gtest/include/**/**/*.h",
        "gtest/include/**/**/**/*.h",
        "gtest/**/*.h"
    ]),
    copts = ["-Iexternal/gtest/gtest/include",
             "-Iexternal/gtest/gtest"],
    linkopts = ["-pthread"],
    visibility = ["//visibility:public"],
)
