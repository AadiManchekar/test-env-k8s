# test-env-k8s
Large Enterprises use a k8s test environment to do their testing be it on dev level or QA level. 
repo contains basic boilerplate code that will help u get started with Creating your own test-environment for your enterprise :)

## Infra Components
To create an ideal test environment, you must have infra components to be up always. We cannot run them as pods since pods may be rescheduled or they might be stuck in containercreating/ Not Ready state due to a lack of resources. We cannot afford this, hence we must operate some core infra components as Docker containers. You can have them dedicated on a node. Make sure that node has a taint so that no other 

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTczNTM1MzIxMiwtMTcyMDA3MDg2NF19
-->