# etcd-tool
Get all the jobs/pods from etcd from etcd, delete jobs/pods that started before [minutes] ago or have been completed.

#Examples:
etcd-tool get pod -i cls-xxx -n default -e http://1.2.3.4:2379 (list pod in the default namespace)
etcd-tool delete job -i cls-xxx -n default -e http://1.2.3.4:2379 -c -m 600 (delete jobs that have been completed and started before 10h ago)
