# deploy-docker-example-voting-app-on-kubernetes-kubernetes
Porject deploying the votting-app application using kubernetes on Google cloud.

you can first create your cluster on Google cloud and once connectes, clone this repository into it.

Important, first run the memory-defaults file so that you can create all the pods without error using the following command:

kubectl apply -f memory-defaults.yaml

![image](https://user-images.githubusercontent.com/107562162/226893585-8c7af79f-4638-49e2-815e-5d68281467d3.png)

Some changes that i noticed are that now it is required to pass the user and password on the postgres pod.

![image](https://user-images.githubusercontent.com/107562162/226894347-21cf62c7-b7d4-42aa-95b1-b4a73f5d90ea.png)

the postgres service can remain the same.

to run the pods and the services, use the command 'kubectl create -f' followed by the file name

once everitihng is running, it will look like this:

the services->

![image](https://user-images.githubusercontent.com/107562162/226898624-2675a09a-02d5-4a8d-b279-5d775e707b35.png)


the pods ->

![image](https://user-images.githubusercontent.com/107562162/226898730-ab1006ed-6f1b-4194-89bc-bb39b5e8a5ab.png)



application running ->

![image](https://user-images.githubusercontent.com/107562162/226898844-4d8e5995-8ac5-4ca4-9f57-0714a6c965d6.png)


![image](https://user-images.githubusercontent.com/107562162/226898914-32fe4dc4-bc4b-41c0-9358-16060349450f.png)
