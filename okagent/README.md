# REQUIREMENTS
- kubernetes >= 1.11
- helm3
# INSTALLATION
- Add okmeter helm repository and get the latest version of okagent helm-chart:
    ```
    helm repo add okmeter https://okmeter.github.io/charts/
    helm pull okmeter/okagent --untar
    ```

- Edit `okagent/values.yaml`. You have to fill `apiToken`
- Install chart to your kubernetes cluster:
    ```
    helm install okagent okagent --create-namespace --namespace okagent`
    ```