cc_binary(
    name = "pcl_bazel_trial",
    srcs = ["main.cpp"],
    copts = [
        "-std=c++14",
        "-I/usr/include/eigen3",
        "-I/usr/include/vtk-6.2",
    ],
    linkopts = [
        "-shared",
    ],
    deps = [
        "@pcl_lib_repo//:pcl_lib",
    ],
)