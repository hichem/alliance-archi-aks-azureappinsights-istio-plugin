
# Azure Application Insights Istio Plugin

This project creates a helm chart for Azure Application Insights Istio Plugin.
The official azure repo is located on Github:
https://github.com/microsoft/Application-Insights-Istio-Adapter

To build the helm chart, install helm and run the following command:

~~~
helm package helm/application-insights-istio-mixer-adapter
~~~

Push the generated chart to azure container registry using the following command:

~~~
az acr login
az acr helm push application-insights-istio-mixer-adapter-0.4.0.tgz  --force
~~~

