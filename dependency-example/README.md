## dependency-example
```sh
$ cd main-chart

$ helm dependency update

$ helm template .
---
# Source: main-chart/charts/sub-chart-1/templates/sub-1-config.yaml
apiVersion: v1
kind: ConfigMap
metadata:
  name: sub-chart-1-config
data:
  foo: piyo
---
# Source: main-chart/charts/sub-chart-2/templates/sub-2-config.yaml
apiVersion: v1
kind: ConfigMap
metadata:
  name: sub-chart-2-config
data:
  bar: piyo
---
# Source: main-chart/charts/sub-chart-3/templates/sub-3-config.yaml
apiVersion: v1
kind: ConfigMap
metadata:
  name: sub-chart-3-config
data:
  piyo: foo
---
# Source: main-chart/templates/main-config.yaml
apiVersion: v1
kind: ConfigMap
metadata:
  name: main-chart-config
data:
  foo: bar
```
