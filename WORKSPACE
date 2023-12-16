load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

RULES_JVM_EXTERNAL_TAG = '4.1'
RULES_JVM_EXTERNAL_SHA = 'f36441aa876c4f6427bfb2d1f2d723b48e9d930b62662bf723ddfb8fc80f0140'

http_archive(
    name = "rules_jvm_external",
    strip_prefix = "rules_jvm_external-%s" % RULES_JVM_EXTERNAL_TAG,
    sha256 = RULES_JVM_EXTERNAL_SHA,
    url = "https://github.com/bazelbuild/rules_jvm_external/archive/%s.zip" % RULES_JVM_EXTERNAL_TAG,
)

load("@rules_jvm_external//:defs.bzl", "maven_install")

maven_install(
    artifacts = [
        "com.fasterxml.jackson.core:jackson-databind:2.15.3",
        "com.google.guava:guava:32.0.1-jre",
        "com.google.protobuf:protobuf-java:3.24.0",
        "io.grpc:grpc-core:1.60.0",
        "org.apache.tomcat.embed:tomcat-embed-core:10.1.16",
        "org.springframework:spring-core:6.1.1",
        "org.springframework.boot:spring-boot:3.2.0",
        "org.springframework.boot:spring-boot-autoconfigure:3.2.0",
        "org.springframework.boot:spring-boot-starter-web:3.2.0",
        "org.yaml:snakeyaml:2.2"
        ],
    repositories = [
        "https://repo1.maven.org/maven2",
    ] )