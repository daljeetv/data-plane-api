load("//bazel:api_build_system.bzl", "api_proto_library")

licenses(["notice"])  # Apache 2

api_proto_library(
    name = "http_connection_manager",
    srcs = ["http_connection_manager.proto"],
    deps = [
        "//api:base",
        "//api:protocol",
        "//api:rds",
        "//api/filter/accesslog:accesslog",
    ],
)

api_proto_library(
    name = "mongo_proxy",
    srcs = ["mongo_proxy.proto"],
    deps = ["//api/filter:fault"],
)

api_proto_library(
    name = "tcp_proxy",
    srcs = ["tcp_proxy.proto"],
    deps = [
        "//api/filter/accesslog:accesslog",
        "//api:address",
    ],
)

api_proto_library(
    name = "redis_proxy",
    srcs = ["redis_proxy.proto"],
)

api_proto_library(
    name = "client_ssl_auth",
    srcs = ["client_ssl_auth.proto"],
    deps = ["//api:address"],
)

api_proto_library(
    name = "rate_limit",
    srcs = ["rate_limit.proto"],
    deps = ["//api:rls"],
)
