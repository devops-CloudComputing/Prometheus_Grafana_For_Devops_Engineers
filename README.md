# Prometheus_Grafana_For_Devops_Engineers
**Introduction:**
In this project we will explore what are monitoring tools, why we need monitoring tools like prometheus, Grafana, how to install and use them to monitor kubernetes cluster.
We will be using minikube kubernetes cluster and use prometheus for monitoring and visualise using grafana.  We will create grafana dashboard which will show API servers, deployment on our cluster, current status of our cluster, replicas etc. 
Lets start with Why? We need tools like prometheus and grafana.
Monitoring your Kubernetes cluster is essential for ensuring the health and performance of your applications and infrastructure. Here are some reasons why monitoring your Kubernetes cluster is important:
Identify issues and troubleshoot: By monitoring your Kubernetes cluster, you can quickly identify issues such as application crashes, resource bottlenecks, and network problems. With real-time monitoring, you can troubleshoot issues before they escalate and impact your users.
Optimize performance and capacity: Monitoring allows you to track the performance of your applications and infrastructure over time, and identify opportunities to optimize performance and capacity. By understanding usage patterns and resource consumption, you can make informed decisions about scaling your infrastructure and improving the efficiency of your applications.
Ensure high availability: Kubernetes is designed to provide high availability for your apply.

**Why Prometheus?**

Prometheus is an open-source monitoring and alerting system that helps you collect and store metrics about your software systems and infrastructure, and analyze that data to gain insights into their health and performance. It provides a powerful query language, a flexible data model, and a range of integrations with other tools and systems. With Prometheus, you can easily monitor metrics such as CPU usage, memory usage, network traffic, and application-specific metrics, and use that data to troubleshoot issues, optimize performance, and create alerts to notify you when things go wrong.

**Why prometheus not other tools?**

Prometheus is a popular choice for Kubernetes monitoring for several reasons:
Open-source: Prometheus is an open-source project that is free to use and has a large community of contributors. This means that you can benefit from ongoing development, bug fixes, and feature enhancements without paying for a commercial monitoring solution.
Native Kubernetes support: Prometheus is designed to work seamlessly with Kubernetes, making it easy to deploy and integrate with your Kubernetes environment. It provides pre-configured Kubernetes dashboards and supports auto-discovery of Kubernetes services and pods.
Powerful query language: Prometheus provides a powerful query language that allows you to easily retrieve and analyze metrics data. This allows you to create custom dashboards and alerts, and to troubleshoot issues more easily.
Scalability: Prometheus is designed to be highly scalable, allowing you to monitor large and complex Kubernetes environments with ease. It supports multi-node architectures and can handle large volumes of data without significant performance degradation.
Integrations: Prometheus integrates with a wide range of other tools and systems, including Grafana for visualization, Alertmanager for alerting, and Kubernetes API server for metadata discovery.

**Prometheus Architecture:**

When you install prometheus there is a component called prometheus server, prometheus server has http server and prometheus server collects all the information of K8s cluster using kubernetes API server. This inbuild K8s server exposes many metrics prometheus store this all info in TSDB (time series data base). We can also prometheus with Alert manager and sent notification to different platforms like slack. 
**Why Grafana?**

Grafana is basically use for visualization, we can display prometheus information is better way using charts and diagrams using grafana. We can configure prometheus as data source and get the information to the grafana we can create some nice charts and diagrams. 
