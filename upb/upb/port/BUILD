# Copyright (c) 2009-2021, Google LLC
# All rights reserved.
#
# Use of this source code is governed by a BSD-style
# license that can be found in the LICENSE file or at
# https://developers.google.com/open-source/licenses/bsd

load("//upb/bazel:build_defs.bzl", "UPB_DEFAULT_COPTS")

cc_library(
    name = "port",
    hdrs = [
        "atomic.h",
        "vsnprintf_compat.h",
    ],
    copts = UPB_DEFAULT_COPTS,
    textual_hdrs = [":inc"],
    visibility = ["//visibility:public"],
)

filegroup(
    name = "inc",
    srcs = [
        "def.inc",
        "undef.inc",
    ],
    visibility = ["//visibility:public"],
)

# begin:github_only
filegroup(
    name = "source_files",
    srcs = glob(
        [
            "**/*.h",
            "**/*.inc",
        ],
    ),
    visibility = [
        "//upb/cmake:__pkg__",
        "//upb/python/dist:__pkg__",
    ]
)
# end:github_only
