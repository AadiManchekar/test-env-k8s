# test-env-k8s
Large Enterprises use a k8s test environment to do their testing be it on dev level or QA level. 
repo contains basic boilerplate code that will help u get started with Creating your own test-environment for your enterprise :)

## Infra Components
To build a perfect test-environment u need to have infra components that are up always. We cannot run them as pods, because there are chances pods get reschedule or is in not ready state due to low resource availability. We cannot afford that hence we have to run some core infra components as a docker container. 

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE3MjAwNzA4NjRdfQ==
-->