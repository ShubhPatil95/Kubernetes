## 1.Pod

![image](https://user-images.githubusercontent.com/74223025/227868417-dc461649-ee79-4dcc-9cf5-197c8b56f603.png)

## 2. Service

![image](https://user-images.githubusercontent.com/74223025/227868862-2e0525ac-d3a2-40be-998a-ab57d12d8b18.png)

## 3. Ingress

![image](https://user-images.githubusercontent.com/74223025/227881173-4152897b-06a3-4fad-8881-53e7afe7d556.png)

Now if you want to connect with your application through browser then you can use URL like: http://ServerIp:NodePort. Here external request will first come to ingress and then ingress will route it to different pods clusters(ClusterIP).

![image](https://user-images.githubusercontent.com/74223025/227869658-12101089-fe07-45a5-95e8-54f0ee4d7547.png)

## 4. ConfigMap
As we know pods communicates with each other using service IP addresses however where will you store those IP addresses? => ConfigMap. It stores the data into plain text formats.

![image](https://user-images.githubusercontent.com/74223025/229040796-6725af3f-bf25-448d-8c1d-522099afeae1.png)

## 5. Secret
Dont put credentials into ConfigMap, Secrets are used to store sensitive information like username and password. It stores the data into encoded format.

![image](https://user-images.githubusercontent.com/74223025/229041019-b1739275-7549-42c1-8916-a8b7c5ec5c9c.png)
