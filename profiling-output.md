1. Ansible operator

Wednesday 02 June 2021  12:22:24 -0700 (0:00:00.587)       0:03:19.034 ********
===============================================================================
Clone the operator-sdk project. ----------------------------------------- 3.26s
Attempt to fix file permissions. ---------------------------------------- 1.09s
Deploy a memcached DaemonSet so image is pulled to all nodes. ----------- 0.04s
Create a Memcached DaemonSet. ------------------------------------------- 6.75s
Delete the Memcached DaemonSet. ----------------------------------------- 1.72s
Deploy cert-manager (required for Go operator). ------------------------- 0.06s
Deploy prometheus-operator (required for metrics service). -------------- 0.05s
Download prometheus-operator manifest. ---------------------------------- 1.25s
Manually create the prometheus-operator ServiceAccount. ----------------- 1.19s
Deploy prometheus-operator into the cluster. --------------------------- 44.97s
Delete prometheus-operator manifest. ------------------------------------ 0.33s
Build, deploy, benchmark, and undeploy operators. ----------------------- 0.08s
Set the ansible memcached operator image name. -------------------------- 0.03s
Set the app label selector for Helm. ------------------------------------ 0.02s
Ensure the operator namespace exists. ----------------------------------- 0.94s
Set the correct subdirectory for the Go operator example. --------------- 0.03s
Build, push, and deploy the ansible memcached operator. ---------------- 11.54s
Wait for Operator Pod to be 'Running'. --------------------------------- 22.40s
Pause to allow cluster to stabilize. ----------------------------------- 10.04s
Deploy 15 ansible memcached CRs. ---------------------------------------- 1.28s
[B1] Wait for 15 ansible Memcached Pods to be running. ----------------- 30.63s
[B1] Wait for ansible Memcached Pods to be ready. ----------------------- 1.70s
Add one more CR to the count. ------------------------------------------- 0.04s
Delete the ansible pod so it restarts. ---------------------------------- 1.62s
Deploy 16 ansible memcached CRs. ---------------------------------------- 1.59s
[B2] Wait for 16 ansible Memcached Pods to be running. ----------------- 33.55s
Un-deploy 16 ansible memcached CRs. ------------------------------------- 2.14s
[B3] Wait for all ansible Memcached Pods to be gone. ------------------- 20.08s
Undeploy the ansible memcached operator. -------------------------------- 0.59s


2. Helm operator

Wednesday 02 June 2021  12:31:22 -0700 (0:00:00.542)       0:05:41.770 ********
===============================================================================
Clone the operator-sdk project. ----------------------------------------- 3.32s
Attempt to fix file permissions. ---------------------------------------- 1.10s
Deploy a memcached DaemonSet so image is pulled to all nodes. ----------- 0.04s
Create a Memcached DaemonSet. ------------------------------------------- 6.69s
Delete the Memcached DaemonSet. ----------------------------------------- 1.08s
Deploy cert-manager (required for Go operator). ------------------------- 0.04s
Deploy prometheus-operator (required for metrics service). -------------- 0.03s
Download prometheus-operator manifest. ---------------------------------- 1.10s
Manually create the prometheus-operator ServiceAccount. ----------------- 0.93s
Deploy prometheus-operator into the cluster. --------------------------- 44.66s
Delete prometheus-operator manifest. ------------------------------------ 0.33s
Build, deploy, benchmark, and undeploy operators. ----------------------- 0.08s
Set the helm memcached operator image name. ----------------------------- 0.03s
Set the app label selector for Helm. ------------------------------------ 0.03s
Ensure the operator namespace exists. ----------------------------------- 0.97s
Set the correct subdirectory for the Go operator example. --------------- 0.03s
Build, push, and deploy the helm memcached operator. ------------------- 19.89s
Wait for Operator Pod to be 'Running'. --------------------------------- 13.42s
Pause to allow cluster to stabilize. ----------------------------------- 10.03s
Deploy 15 helm memcached CRs. ------------------------------------------- 1.07s
[B1] Wait for 15 helm Memcached Pods to be running. -------------------- 68.55s
[B1] Wait for helm Memcached Pods to be ready. -------------------------- 4.76s
Add one more CR to the count. ------------------------------------------- 0.03s
Delete the helm pod so it restarts. ------------------------------------- 0.99s
Deploy 16 helm memcached CRs. ------------------------------------------- 1.31s
[B2] Wait for 16 helm Memcached Pods to be running. ------------------- 116.32s
Un-deploy 16 helm memcached CRs. ---------------------------------------- 1.21s
[B3] Wait for all helm Memcached Pods to be gone. ---------------------- 43.16s
Undeploy the helm memcached operator. ----------------------------------- 0.54s
