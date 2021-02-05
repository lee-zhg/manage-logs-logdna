# Manage logs with LogDNA in IBM Cloud

`IBM Log Analysis with LogDNA` allows you to capture your application and environment logs, filter out noisy or irrelevant log lines, alert, search, and archive your log data. You can build real-time dashboards with highly interactive graphs, including Counters, Gauges, Tables, and Time-Shifted Graphs.

This exercise shows how the `IBM Log Analysis with LogDNA` service can be used to configure and access logs of a Kubernetes application that is deployed on IBM Cloud. You will deploy a Spring Java application to a cluster provisioned on IBM Cloud Kubernetes Service, configure a LogDNA agent, generate application logs and access worker logs, pod logs or network logs. Then, you will search, filter and visualize those logs through Log Analysis with LogDNA Web UI.

Adopted from repo [Spring PetClinic Microservice example running on Kubernetes(in Korean)](https://github.com/hongjsk/spring-petclinic-kubernetes) and [Analyze logs and monitor application health with LogDNA and Sysdig](https://cloud.ibm.com/docs/solution-tutorials?topic=solution-tutorials-application-log-analysis).


## Pre-requisites

* an IBM Cloud account
* a Kubernetes cluster running in IBM cloud (IKS)

> Note: it's highly recommended to enable `private endpoints` (or private service endpoint) when you create your Kubernetes cluster in IBM Cloud. The `private endpoints` can also be enabled after the cluster is created. This provides the option to use the `private endpoints` when configuring LogDNA to collect logs from your application deployed to IKS cluster.

!["iks_private_endpoints"](doc/images/iks_private_endpoints.png)


## Sample application architecture

A simplified version of `petclinic` application is used in this repo. It includes four microservice components.
  * api-gateway
  * customers
  * vets
  * visits

!["iks_private_endpoints"](doc/images/petclinic_architecture.png)

The complete version of `petclinic` application with microservice architecture is available [here](https://github.com/spring-petclinic/spring-petclinic-microservices).


## Exercise Steps

  * Lab 1 - [Prepare exercise environment](README-preparation.md)
  * Lab 2 - [Deploy sample application to IKS cluster](README-deploy-app.md)
  * Lab 3 - []()
  * Lab 4 - []()


## Related Links

There is lots of great information, tutorials, articles, etc on the [IBM Developer site](https://developer.ibm.com) as well as broader web. Here are a subset of good examples related to data understanding, visualization and processing:

- [Build ML Model for Loan Eligibility using Modeler](https://developer.ibm.com/tutorials/predict-loan-eligibility-using-jupyter-notebook-ibm-spss-modeler/)
- [Build ML Model to predict Chuurn](https://developer.ibm.com/patterns/predict-customer-churn-using-watson-studio-and-jupyter-notebooks/)
- [Predict Fraud with Skewed Data](https://developer.ibm.com/patterns/predicting-fraud-using-skewed-data/)
- [XGBoost Model on Client Purchases](https://developer.ibm.com/patterns/analyze-bank-marketing-data-using-xgboost-gain-insights-client-purchases/)
- [ML Model on Medical Data](https://developer.ibm.com/patterns/analyze-open-medical-data-sets-to-gain-insights/)


## General Links

- [IBM Developer](https://developer.ibm.com)
- [Watson Studio](https://dataplatform.ibm.com/)
- [Watson Studio Overview](https://dataplatform.cloud.ibm.com/docs/content/wsj/getting-started/overview-ws.html?audience=wdp&context=wdp&linkInPage=true)
- [Watson Machine Learning Python SDK](https://wml-api-pyclient.mybluemix.net/)
- [Watson Studio Video Learning Center](https://www.youtube.com/playlist?list=PLzpeuWUENMK3u3j_hffhNZX3-Jkht3N6V)
- [Data Science Code Patterns](https://developer.ibm.com/code/technologies/data-science/)
