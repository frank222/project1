cc_binary(
	name = "main",
	srcs = ["hello.cc"]
)

cc_test(
    name = "lib_test",
    srcs = ["lib_test.cc"],
#    copts = ["-Iexternal/gtest/gtest/include"],
    copts = ["-Iexternal/gtest/googletest-release-1.8.0/googletest/include"],
    deps = [
#	":gtest_main",
        "@gtest//:main",
#        "//external:gtest_local/main",
    ],
)

