You delete a Pod
        │
        ▼
API Server updates etcd
        │
        ▼
Controller Manager notices:
Desired = 3
Current = 2
        │
        ▼
ReplicaSet creates a new Pod object
        │
        ▼
Scheduler selects the best Worker Node
        │
        ▼
Kubelet on that Worker Node starts the Pod
        │
        ▼
Container Runtime starts the container
