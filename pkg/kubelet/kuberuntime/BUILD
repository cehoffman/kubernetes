package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_library(
    name = "go_default_library",
    srcs = [
        "doc.go",
        "fake_kuberuntime_manager.go",
        "helpers.go",
        "instrumented_services.go",
        "kuberuntime_container.go",
        "kuberuntime_gc.go",
        "kuberuntime_image.go",
        "kuberuntime_logs.go",
        "kuberuntime_manager.go",
        "kuberuntime_sandbox.go",
        "labels.go",
        "legacy.go",
        "security_context.go",
    ],
    tags = ["automanaged"],
    deps = [
        "//pkg/api:go_default_library",
        "//pkg/api/v1:go_default_library",
        "//pkg/api/v1/ref:go_default_library",
        "//pkg/credentialprovider:go_default_library",
        "//pkg/kubelet/api:go_default_library",
        "//pkg/kubelet/api/v1alpha1/runtime:go_default_library",
        "//pkg/kubelet/container:go_default_library",
        "//pkg/kubelet/dockertools:go_default_library",
        "//pkg/kubelet/events:go_default_library",
        "//pkg/kubelet/images:go_default_library",
        "//pkg/kubelet/lifecycle:go_default_library",
        "//pkg/kubelet/metrics:go_default_library",
        "//pkg/kubelet/network:go_default_library",
        "//pkg/kubelet/prober/results:go_default_library",
        "//pkg/kubelet/qos:go_default_library",
        "//pkg/kubelet/types:go_default_library",
        "//pkg/kubelet/util/cache:go_default_library",
        "//pkg/kubelet/util/format:go_default_library",
        "//pkg/security/apparmor:go_default_library",
        "//pkg/securitycontext:go_default_library",
        "//pkg/util/parsers:go_default_library",
        "//pkg/util/selinux:go_default_library",
        "//pkg/util/tail:go_default_library",
        "//pkg/util/version:go_default_library",
        "//vendor/github.com/armon/circbuf:go_default_library",
        "//vendor/github.com/docker/docker/pkg/jsonlog:go_default_library",
        "//vendor/github.com/fsnotify/fsnotify:go_default_library",
        "//vendor/github.com/golang/glog:go_default_library",
        "//vendor/github.com/google/cadvisor/info/v1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/types:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/errors:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/runtime:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/sets:go_default_library",
        "//vendor/k8s.io/client-go/tools/record:go_default_library",
        "//vendor/k8s.io/client-go/util/flowcontrol:go_default_library",
    ],
)

go_test(
    name = "go_default_test",
    srcs = [
        "helpers_test.go",
        "kuberuntime_container_test.go",
        "kuberuntime_gc_test.go",
        "kuberuntime_image_test.go",
        "kuberuntime_logs_test.go",
        "kuberuntime_manager_test.go",
        "kuberuntime_sandbox_test.go",
        "labels_test.go",
    ],
    library = ":go_default_library",
    tags = ["automanaged"],
    deps = [
        "//pkg/api/v1:go_default_library",
        "//pkg/apis/componentconfig:go_default_library",
        "//pkg/kubelet/api/testing:go_default_library",
        "//pkg/kubelet/api/v1alpha1/runtime:go_default_library",
        "//pkg/kubelet/container:go_default_library",
        "//pkg/kubelet/container/testing:go_default_library",
        "//pkg/kubelet/network:go_default_library",
        "//pkg/kubelet/network/testing:go_default_library",
        "//vendor/github.com/golang/mock/gomock:go_default_library",
        "//vendor/github.com/google/cadvisor/info/v1:go_default_library",
        "//vendor/github.com/stretchr/testify/assert:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/types:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/intstr:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/sets:go_default_library",
        "//vendor/k8s.io/client-go/util/flowcontrol:go_default_library",
    ],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [":package-srcs"],
    tags = ["automanaged"],
)
