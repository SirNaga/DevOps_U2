# Scaling Strategy - Horizontal Pod Autoscaler

The file HorizontalPodAutoscaler.yaml consists the configuration for the scaling strategy.

Trigger: CPU

The scaling mechanism triggers on CPU usage. If the average CPU usage is above 50% it will create a new pod.

To assert the functionality a load generator and cli was used. To generat the load to reach the threshold jmeter was used. To see the autoscaling I used the ``````kubectl get hpa``````  command. This command shows you the current CPU usage and the amount of replicas.