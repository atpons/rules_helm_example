# rules_helm_example

This repository shows example use of the [atpons/rules_helm](https://github.com/atpons/rules_helm) (forked) Bazel build
rules.

**atpons/rules_helm differs from [tmc/rules_helm](https://github.com/tmc/rules_helm) in that `context` can be specified and is compatible with Helm 3.**

Examples:
* `bazel run //:test_chart_1.install` this will install the chart defined in BUILD to the currently configured kubernetes cluster with specified context.
* `bazel run //charts/istio:istio_init.install` and `bazel run //charts/istio:istio.install` will install Istio.
