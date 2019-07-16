new_local_repository (
    name = "pcl_lib_repo",
    path = "/usr/local/include/pcl-1.9",
    build_file_content = """
package(default_visibility = ["//visibility:public"])
cc_library(
    name = "pcl_lib",
    defines = ["DISABLE_PCAP", "DISABLE_PNG", "DISABLE_LIBUSB_1_0", "DISABLE_QHULL"],
    includes = ["."],
    hdrs = glob([ "pcl/**/*.h", "pcl/**/*.hpp"]),
    alwayslink = True,
    linkopts = [
        "-L/usr/local/lib",
        "-lpcl_common",
        "-lpcl_features",
        "-lpcl_filters",
        "-lpcl_io_ply",
        "-lpcl_io",
        "-lpcl_kdtree",
        "-lpcl_keypoints",
        "-lpcl_octree",
        "-lpcl_outofcore",
        "-lpcl_people",
        "-lpcl_recognition",
        "-lpcl_registration",
        "-lpcl_sample_consensus",
        "-lpcl_search",
        "-lpcl_segmentation",
        "-lpcl_surface",
        "-lpcl_tracking",
        "-lpcl_visualization",
    ],
    visibility = ["//visibility:public"],
)
""",
)