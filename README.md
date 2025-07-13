# kubernetes_project

OBJECTIVES :
In this Practice Project, I have build and deploy a JavaScript application to Kubernetes using Docker.
By creating the following:
.ConfigMap
.DaemonSet
.Kubernetes Service
.Secret
.Volumes and Persistent Volume Claims


TASK 1
1. Built the docker images :
   <img width="1518" height="936" alt="image" src="https://github.com/user-attachments/assets/753899d1-c94c-414a-bab6-619544cad7e0" />

2. after applying the deployment :
   <img width="1546" height="217" alt="image" src="https://github.com/user-attachments/assets/e58c9162-0094-4c0a-b9c3-64e404f7054a" />

3. Push the tagged image to the IBM Cloud container registry.
  <img width="887" height="473" alt="image" src="https://github.com/user-attachments/assets/6f888b6e-a6da-4546-a022-77c3f5e3953b" />
4. listing all the images present in the cloud after the image creation :
   <img width="861" height="450" alt="image" src="https://github.com/user-attachments/assets/2f395b4d-426c-499d-82a8-ef5173b94f26" />
5. The first output from the deployed app :
   <img width="1918" height="1152" alt="image" src="https://github.com/user-attachments/assets/da4e09e3-cc6d-409d-bf04-6f3d4934f9b2" />
    <img width="777" height="545" alt="image" src="https://github.com/user-attachments/assets/5cd858db-9d21-4d7d-a090-19ba4e028a75" />
6.  the successful creation of the ConfigMap :
     <img width="686" height="300" alt="image" src="https://github.com/user-attachments/assets/59fa1920-d9ae-4329-b668-dd99537fef7f" />
7. <img width="717" height="238" alt="image" src="https://github.com/user-attachments/assets/29c930a5-ba02-4011-a42e-b066cf5e813b"/>

TYPE: NodePort: It specifies that this service is of type NodePort, meaning it exposes the service on a port on all nodes in the cluster.

CLUSTER-IP: 172.21.26.244: This is the internal Cluster IP address assigned to the service. It is used for communication within the Kubernetes cluster.

EXTERNAL-IP: <none>: It indicates that there is no external IP address assigned to this service. External clients cannot directly access this service from outside the Kubernetes cluster.

PORT(S): 80:30016/TCP: This indicates that port 80 is exposed internally by the service, and externally it is accessible on port 30016 using the TCP protocol. The format is externalPort/protocol.

AGE: 25s: It shows that the service has been running for 25 seconds since its creation.

Note : Based on the availability of Cluster-IP addresses or ports this value may differ in your lab Environment.

8. TASK2 : DaemonSets
9. I'VE  created a DaemonSet to ensure that a pod runs on each node in the cluster, including the nodes where the 'myapp' pods are deployed. Creating a DaemonSet enhances the availability and fault tolerance of your application (myapp) by ensuring that it runs on every node in the cluster, providing redundancy and load distribution.
<img width="707" height="185" alt="image" src="https://github.com/user-attachments/assets/c033b101-b723-4b31-9075-b5dc281b06cc" />


TASK 3:
In this Task, I have created a Kubernetes Service to expose the application within the cluster.
  <img width="1033" height="152" alt="image" src="https://github.com/user-attachments/assets/0ef76a61-3b02-47af-a97c-23f650c8913b" />

TASK 4 :
In this task, I've showed how to create and manage secrets in Kubernetes to securely store sensitive information, such as passwords, tokens, and SSH keys.
<img width="863" height="197" alt="image" src="https://github.com/user-attachments/assets/c1a9b2ed-f65d-4d7a-a2d5-f4296d60a0c7" />

TASK 5: Volumes and persistent volume claims
In this task, i have showed how to define volumes and persistent volume claims (PVCs) in Kubernetes to provide storage for your application.

<img width="940" height="757" alt="image" src="https://github.com/user-attachments/assets/d733dbb6-c2d6-47bf-a688-a3866d342205" />




Conclusion
In this Practice Project, I have started by building and deploying a Javascript application to Kubernetes using Docker.
I further created and understood a ConfigMap to manage configuration data for the application, a DaemonSet to ensure that a pod runs on each node in the cluster, a Kubernetes Service to expose MY application within the cluster, and a Secret to securely store sensitive information.
Further, I explored how to define volumes and persistent volume claims to provide storage for my application.

