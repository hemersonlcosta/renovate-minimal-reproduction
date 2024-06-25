# 29813

[Reproduction for ](https://github.com/renovatebot/renovate/discussions/29813#discussioncomment-9864439).

## Current behavior

I'm facing trouble with the "k8s-events-forwarder" image version, which is a dependency from the nri-kube-events chart. When configuring the regexManagers to obtain the Docker image version, it pulls the latest version (1.53.0), rather than the correct version (1.52.3) indicated in the values file on [link ](https://github.com/newrelic/nri-kube-events/blob/v2.9.10/charts/nri-kube-events/values.yaml).

This is reference where is the string export NEWRELIC_K8S_EVENT_FORWARDER_TAG="1.52.0" in newrelic/newrelic-initialize-variables.sh.


## Expected behavior

It must search from `nri-kube-events` the dependency version of item `k8s-events-forwarder` in this case `1.52.3`.

## Link to the Renovate issue or Discussion

[Link Discussion here.](https://github.com/renovatebot/renovate/discussions/29813#discussioncomment-9864439).
