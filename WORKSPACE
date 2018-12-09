## Copyright 2018 The Closure Compiler Authors. All rights reserved.
##
## Licensed under the Apache License, Version 2.0 (the "License");
## you may not use this file except in compliance with the License.
## You may obtain a copy of the License at
##
##    http://www.apache.org/licenses/LICENSE-2.0
##
## Unless required by applicable law or agreed to in writing, software
## distributed under the License is distributed on an "AS IS" BASIS,
## WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
## See the License for the specific language governing permissions and
## limitations under the License.

workspace(name = "com_google_closure_compiler")

load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "bazel_skylib",
    strip_prefix = "bazel-skylib-master",
    urls = [
        "https://github.com/bazelbuild/bazel-skylib/archive/master.zip",
    ],
)

http_archive(
    name = "com_google_protobuf",
    strip_prefix = "protobuf-master",
    urls = [
        "https://github.com/protocolbuffers/protobuf/archive/master.zip",
    ],
)

http_archive(
    name = "io_bazel_rules_closure",
    strip_prefix = "rules_closure-bazel",
    urls = [
        "https://github.com/Yannic/rules_closure/archive/bazel.zip",
    ],
)

# LICENSE: The Apache Software License, Version 2.0
maven_jar(
    name = "args4j",
    artifact = "args4j:args4j:2.0.26",
    sha1 = "01ebb18ebb3b379a74207d5af4ea7c8338ebd78b",
)

# LICENSE: The Apache Software License, Version 2.0
maven_jar(
    name = "gson",
    artifact = "com.google.code.gson:gson:jar:2.8.1",
    sha1 = "02a8e0aa38a2e21cb39e2f5a7d6704cbdc941da0",
)

# LICENSE: The Apache Software License, Version 2.0
maven_jar(
    name = "guava",
    artifact = "com.google.guava:guava:25.1-jre",
    sha1 = "6c57e4b22b44e89e548b5c9f70f0c45fe10fb0b4",
)

# LICENSE: The Apache Software License, Version 2.0
maven_jar(
    name = "guava_testlib",
    artifact = "com.google.guava:guava-testlib:25.1-jre",
    sha1 = "1ec77c45666cf17da76cd80725194148a8ffc440",
)

# LICENSE: The Apache Software License, Version 2.0
maven_jar(
    name = "jsr305",
    artifact = "com.google.code.findbugs:jsr305:3.0.1",
    sha1 = "f7be08ec23c21485b9b5a1cf1654c2ec8c58168d",
)

# LICENSE: Common Public License 1.0
maven_jar(
    name = "junit",
    artifact = "junit:junit:4.11",
    sha1 = "4e031bb61df09069aeb2bffb4019e7a5034a4ee0",
)

# LICENSE: The Apache Software License, Version 2.0
maven_jar(
    name = "truth",
    artifact = "com.google.truth:truth:0.41",
    sha1 = "846cd094934911f635ba2dadc016d538b8c30927",
)

# LICENSE: The Apache Software License, Version 2.0
maven_jar(
    name = "error_prone_annotations",
    artifact = "com.google.errorprone:error_prone_annotations:2.3.1",
    sha1 = "a6a2b2df72fd13ec466216049b303f206bd66c5d",
)

# LICENSE: The Apache Software License, Version 2.0
maven_jar(
    name = "mockito",
    artifact = "org.mockito:mockito-core:1.9.5",
    sha1 = "c3264abeea62c4d2f367e21484fbb40c7e256393",
)

# LICENSE: The Apache Software License, Version 2.0
# Required by mockito
maven_jar(
    name = "objenesis",
    artifact = "org.objenesis:objenesis:1.0",
    sha1 = "9b473564e792c2bdf1449da1f0b1b5bff9805704",
)

load("@io_bazel_rules_closure//closure:defs.bzl", "closure_repositories")

closure_repositories(
    omit_com_google_javascript_closure_compiler = True,
    omit_com_google_protobuf = True,
)
