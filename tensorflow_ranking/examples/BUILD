# Description:
# TensorFlow Ranking examples.

# Placeholder for internal Python version compatibility macro.

package(
    default_visibility = [
        "//tensorflow_ranking:__subpackages__",
    ],
)

licenses(["notice"])  # Apache 2.0

exports_files(["LICENSE"])

py_library(
    name = "tf_ranking_libsvm_lib",
    srcs = ["tf_ranking_libsvm.py"],
    srcs_version = "PY2AND3",
    deps = [
        # py/absl/flags dep,
        # py/tensorflow dep,
        "//tensorflow_ranking",
    ],
)

py_binary(
    name = "tf_ranking_libsvm_py_binary",
    srcs = ["tf_ranking_libsvm.py"],
    main = "tf_ranking_libsvm.py",
    python_version = "PY3",
    srcs_version = "PY2AND3",
    deps = [
        ":tf_ranking_libsvm_lib",
    ],
)

py_test(
    name = "tf_ranking_libsvm_test",
    size = "large",
    srcs = ["tf_ranking_libsvm_test.py"],
    srcs_version = "PY2AND3",
    tags = [
        "no_pip",
        "notsan",
    ],
    deps = [
        ":tf_ranking_libsvm_lib",
        # py/absl/flags dep,
        # py/absl/testing:flagsaver dep,
        # py/absl/testing:parameterized dep,
        # py/tensorflow dep,
    ],
)

py_library(
    name = "tf_ranking_tfrecord_lib",
    srcs = ["tf_ranking_tfrecord.py"],
    srcs_version = "PY2AND3",
    deps = [
        # py/absl/flags dep,
        # py/tensorflow dep,
        "//tensorflow_ranking",
    ],
)

py_binary(
    name = "tf_ranking_tfrecord_py_binary",
    srcs = ["tf_ranking_tfrecord.py"],
    main = "tf_ranking_tfrecord.py",
    python_version = "PY3",
    srcs_version = "PY2AND3",
    deps = [
        ":tf_ranking_tfrecord_lib",
    ],
)

py_test(
    name = "tf_ranking_tfrecord_test",
    size = "large",
    srcs = ["tf_ranking_tfrecord_test.py"],
    srcs_version = "PY2AND3",
    tags = [
        "no_pip",
        "notsan",
    ],
    deps = [
        ":tf_ranking_tfrecord_lib",
        # py/absl/flags dep,
        # py/absl/testing:flagsaver dep,
        # py/absl/testing:parameterized dep,
        # py/tensorflow dep,
        # tensorflow_serving/apis:input_proto_py_pb2 dep,
    ],
)
