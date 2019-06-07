load("@npm_bazel_typescript//:defs.bzl", "ts_library")
load("@build_bazel_rules_nodejs//:defs.bzl", "nodejs_binary")

ts_library(
    name = "ts",
    srcs = ["main.ts"],
)

nodejs_binary(
    name = "bin",
    data = [
      ":ts",
    ],
    entry_point = "tools_evertz_buildops/ts/main.js",
)
