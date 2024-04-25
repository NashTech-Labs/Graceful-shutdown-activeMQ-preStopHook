# Apache ActiveMQ StatefulSet Helm Chart

This Helm chart deploys an Apache ActiveMQ StatefulSet on your Kubernetes cluster with Graceful shutdown preStop Hook.

## Prerequisites

- Helm must be installed on your machine.
- A Kubernetes cluster must be available.
- Ensure you have the necessary permissions to deploy resources in your Kubernetes cluster.

## Installation

1. **Clone the Helm Chart**

    ```bash
    git clone https://github.com/NashTech-Labs/Graceful-shutdown-activeMQ-preStopHook.git
    cd Graceful-shutdown-activeMQ-preStopHook
    ```

2. **Install the Chart**

    To install the chart, run the following command:

    ```bash
    helm install <release_name> .
    ```

    Replace `<release_name>` with a unique name for the release.

3. **Monitor the Deployment**

    After installation, monitor the deployment to ensure all resources are created successfully:

    ```bash
    kubectl get statefulsets,pods,services
    ```

4. **Upgrade the Chart (Optional)**

    If you need to make changes to your deployment, you can upgrade the chart using the following command:

    ```bash
    helm upgrade <release_name> .
    ```

5. **Rollback the Chart (Optional)**

    In case of any issues, you can rollback to a previous release using the command:

    ```bash
    helm rollback <release_name> <revision>
    ```

## Uninstall the Chart

To uninstall the chart and remove all resources:

```bash
helm uninstall <release_name>
```
