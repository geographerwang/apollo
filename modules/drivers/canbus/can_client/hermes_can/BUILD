load("//tools:cpplint.bzl", "cpplint")

package(default_visibility = ["//visibility:public"])

cc_library(
    name = "hermes_can_client",
    srcs = [
        "hermes_can_client.cc",
    ],
    hdrs = [
        "hermes_can_client.h",
        "bcan.h",
        "bcan_defs.h",
    ],
    deps = [
        "//modules/drivers/canbus/can_client",
        "//third_party/can_card_library/hermes_can",
    ],
)

cc_test(
    name = "hermes_can_client_test",
    size = "small",
    srcs = [
        "hermes_can_client_test.cc",
    ],
    deps = [
        "//modules/common:log",
        "//modules/drivers/canbus/can_client/hermes_can:hermes_can_client",
        "//modules/drivers/canbus/common:canbus_common",
        "@gtest//:main",
    ],
)

cpplint()
