# LSM algorithm methods.

licenses(["notice"])

package(default_visibility = ["//tf_quant_finance:__subpackages__"])

py_library(
    name = "lsm",
    srcs = ["lsm.py"],
    srcs_version = "PY3",
    deps = [
        # tensorflow dep,
    ],
)

py_test(
    name = "lsm_test",
    size = "medium",
    timeout = "moderate",
    srcs = ["lsm_test.py"],
    python_version = "PY3",
    shard_count = 3,
    deps = [
        ":lsm",
        ":payoff",
        # numpy dep,
        # tensorflow dep,
    ],
)

py_library(
    name = "payoff",
    srcs = ["payoff.py"],
    srcs_version = "PY3",
    deps = [
        # tensorflow dep,
    ],
)

py_test(
    name = "payoff_test",
    size = "small",
    srcs = ["payoff_test.py"],
    python_version = "PY3",
    deps = [
        ":payoff",
        # numpy dep,
        # tensorflow dep,
    ],
)
