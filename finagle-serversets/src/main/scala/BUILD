scala_library(
    sources = ["**/*.scala"],
    provides = scala_artifact(
        org = "com.twitter",
        name = "finagle-serversets",
        repo = artifactory,
    ),
    # Exposes a service-loaded class.
    scope = "forced",
    dependencies = [
        "3rdparty/jvm/com/fasterxml/jackson/core:jackson-databind",
        "3rdparty/jvm/com/github/ben-manes/caffeine",
        "3rdparty/jvm/com/google/inject:guice",
        "3rdparty/jvm/org/apache/thrift:libthrift",
        "3rdparty/jvm/org/apache/zookeeper:zookeeper-client",
        "finagle/finagle-core/src/main/scala",
        "finagle/finagle-partitioning/src/main/scala",
        "finagle/finagle-serversets/src/main/java",
        "finagle/finagle-serversets/src/main/resources",
        "finagle/finagle-serversets/src/main/thrift:thrift-java",
        "util/util-app/src/main/scala",
        "util/util-cache",
        "util/util-core/src/main/scala",
        "util/util-logging/src/main/scala",
        "util/util-stats/src/main/scala",
    ],
    exports = [
        "finagle/finagle-partitioning/src/main/scala",
        "util/util-core/src/main/scala",
    ],
)
