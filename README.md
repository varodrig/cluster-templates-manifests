# cluster-templates-manifests
Contains demo manifests used by [cluster-templates-operator](https://github.com/stolostron/cluster-templates-operator/)

There are two types of manifests:
 - **Day1:** define how the cluster needs to be installed
 - **Day2:** define what should be installed on the cluster, once installed

## Manifests
### Day1
 - **hypershift-template:** A hypershift template with NO WORKER nodes. No workload can be run on clusters created from this template. Its only for educational purposes to try the infrastructure out.
 - **hypershift-kubevirt-template:** A template which installs clusters with hypershift control plane and workers on kubevirt virtual machines running on the same cluster.

### Day2:
 - **backstage:** Installs backstage on a cluster.

## How to use
If you install the [cluster-templates-operator](https://github.com/stolostron/cluster-templates-operator/), it already comes with this repository configured.

## How to customize
You can not directly customize the content of this repository. On the other hand, it is a great starting point to create your own custom set of manifersts for your custom templates. To get started from this repository:
 1. Fork this repository
 2. In your fork, go to settings -> pages -> under branch pick main -> click Save
 3. Wait until the pages get live (takes about a minute)
 4. Make sure they are live by visiting the https://`your github user name`.github.io/cluster-templates-manifests 
 5. Now you are ready use your own fork in your setup. If you use the UI, go to Infrastructure -> Cluster templates -> Repositories -> Add a repository -> Helm - paste https://`your github user name`.github.io/cluster-templates-manifests into the Repository URL

# License

Copyright 2022.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

