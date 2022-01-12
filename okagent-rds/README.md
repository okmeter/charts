# REQUIREMENTS
- kubernetes >= 1.11
- helm3
# INSTALLATION
- Add okmeter helm repository and get the latest version of okagent helm-chart:
    ```
    helm repo add okmeter https://okmeter.github.io/charts/
    helm pull okmeter/okagent-rds --untar
    ```

- Edit `okagent/values.yaml`. You have to fill `apiToken` and define the RDS configuration
- Install chart to your kubernetes cluster:
    ```
    helm install okagent-rds okagent-rds --create-namespace --namespace okagent-rds
    ```
