load("//tensorboard/defs:web.bzl", "tf_web_library", "tf_web_test")

package(
    default_testonly = True,
    default_visibility = ["//tensorboard:internal"],
)

licenses(["notice"])  # Apache 2.0

tf_web_test(
    name = "test",
    src = "/vz-projector/test/tests.html",
    web_library = ":test_web_library",
)

tf_web_library(
    name = "test_web_library",
    srcs = [
        "assert.ts",
        "data-provider_test.ts",
        "data_test.ts",
        "sptree_test.ts",
        "tests.html",
        "util_test.ts",
        # "scatterPlotRectangleSelector_test.ts",
        # "vz-projector-projections-panel_test.ts",
    ],
    path = "/vz-projector/test",
    deps = [
        "//tensorboard/components/tf_imports:polymer",
        "//tensorboard/components/tf_imports:web_component_tester",
        "//tensorboard/plugins/projector/vz_projector",
    ],
)
