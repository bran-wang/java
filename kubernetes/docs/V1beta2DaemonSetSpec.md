
# V1beta2DaemonSetSpec

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**minReadySeconds** | **Integer** | The minimum number of seconds for which a newly created DaemonSet pod should be ready without any of its container crashing, for it to be considered available. Defaults to 0 (pod will be considered available as soon as it is ready). |  [optional]
**revisionHistoryLimit** | **Integer** | The number of old history to retain to allow rollback. This is a pointer to distinguish between explicit zero and not specified. Defaults to 10. |  [optional]
**selector** | [**V1LabelSelector**](V1LabelSelector.md) | A label query over pods that are managed by the daemon set. Must match in order to be controlled. If empty, defaulted to labels on Pod template. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/#label-selectors |  [optional]
**template** | [**V1PodTemplateSpec**](V1PodTemplateSpec.md) | An object that describes the pod that will be created. The DaemonSet will create exactly one copy of this pod on every node that matches the template&#39;s node selector (or on every node if no node selector is specified). More info: https://kubernetes.io/docs/concepts/workloads/controllers/replicationcontroller#pod-template | 
**updateStrategy** | [**V1beta2DaemonSetUpdateStrategy**](V1beta2DaemonSetUpdateStrategy.md) | An update strategy to replace existing DaemonSet pods with new pods. |  [optional]



