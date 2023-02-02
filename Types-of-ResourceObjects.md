Kubernetes supports several types of objects for defining, creating, and managing resources in a cluster, including:

Pods: The smallest deployable units in a Kubernetes cluster, consisting of one or more containers.
Replication Controllers: Ensure that a specified number of replicas of a Pod are running at all times. 
Services: Provide network connectivity to Pods.
Deployments: Declarative management for Replication Controllers and Pods. 
Namespaces: Divide cluster resources into virtual clusters isolated from each other, with independent access control and networking.
Roles and RoleBindings: Provide fine-grained access control to cluster resources, allowing you to grant or deny permissions to specific users, groups, or service accounts. 
Custom Resource Definitions (CRDs): Enable the creation of custom resources to extend the Kubernetes API. 