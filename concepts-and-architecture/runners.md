---
description: What are Testground runners?
---

# Runners

A **runner** is a component that takes _**build artifact**_ produced by a [Builder](builders-1.md), and schedules a test run of a test case within the test plan, on the Testground deployment, with the specified number of instances and test parameters.

```text
                                                          ☟
-------------    -----------    ------------------    ----------    ---------------
| plan code | -> | builder | -> | build artifact | -> | runner | -> | test output |
-------------    -----------    ------------------    ----------    ---------------
```

### Supported runners

| builder | input work unit | Environment |
| :--- | :--- | :--- |
| `local:exec` | os-specific executable | local |
| `local:docker` | docker image | local docker environment |
| `cluster:k8s` | docker image | [Kubernetes cluster](../runner-library/cluster-k8s/how-to-create-a-kubernetes-cluster-for-testground.md) |


