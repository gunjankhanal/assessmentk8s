# assessmentk8s

# Step 1: Install Minikube/Kind/k3s or Kubeadm on your ease

Here we have installed Minikube:
And started the service as: minikube start

Installation Script:
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
sudo install minikube-linux-amd64 /usr/local/bin/minikube
 ![image](https://github.com/gunjankhanal/assessmentk8s/assets/20742236/6bb29a61-7fa6-407c-b4d3-37b4b1141f38)

# STEP 2: Clone the Repo from https://github.com/gunjankhanal/assessmentk8s.git as
 ![image](https://github.com/gunjankhanal/assessmentk8s/assets/20742236/20f5376f-af56-40d0-bc6c-fc56941c7ea0)


# STEP 3: CREATE NAMESPACE Django-todo-app
Here our deployment will be on namespace: Django-todo-app
(We can also create it declaratively by creating a namespace.yaml file)
![image](https://github.com/gunjankhanal/assessmentk8s/assets/20742236/e97ad5fd-7581-4b0c-acf6-6a5e20160d7c)


# STEP 4: The deployment.yaml manifest look like this.
![image](https://github.com/gunjankhanal/assessmentk8s/assets/20742236/c3be0c9b-79d1-40f0-8073-e380a54cc333)


# STEP 5: We create a deployment with the command as:
Kubectl create or kubectl apply as:
kubectl apply -f deployment.yaml
![image](https://github.com/gunjankhanal/assessmentk8s/assets/20742236/ca45986c-0981-4c56-a578-f10e776345e2)

 
# STEP 6: Lets see the containers which are running as per the command applied before.
Apart from the system pods, we can see two more pods in –namespace Django-todo-app has been created.
![image](https://github.com/gunjankhanal/assessmentk8s/assets/20742236/e5cdb993-5384-45ed-ac4b-79eb005bef4d)


# STEP 7: Lets Inspect what is going on in the background: 
It can be seen that the image is being pulled in the background.
![image](https://github.com/gunjankhanal/assessmentk8s/assets/20742236/f5cc4f34-f713-455f-82eb-2ce5e2a3203e)
![image](https://github.com/gunjankhanal/assessmentk8s/assets/20742236/33332402-f2e9-4ed1-86af-dfa53d9e1f7f)
![image](https://github.com/gunjankhanal/assessmentk8s/assets/20742236/019ad1ca-26ee-4330-a80d-2efaa3c3979f)



# STEP 8: It can be seen that the image has been pulled.
 ![image](https://github.com/gunjankhanal/assessmentk8s/assets/20742236/a2692519-686d-4507-941e-b94cb429c95e)


# STEP 9: Initially I have service as LoadBalancer. Later I changed it to the type: NodePort making the nodePort to 30007.
 ![image](https://github.com/gunjankhanal/assessmentk8s/assets/20742236/e3835493-aa32-45fe-99f8-2eecd4a081a8)
![image](https://github.com/gunjankhanal/assessmentk8s/assets/20742236/94e72650-b032-46b5-9a4a-dd4b41dd0f54)
![image](https://github.com/gunjankhanal/assessmentk8s/assets/20742236/81c82871-aabf-4c6a-b5cd-55058c1ff0b4)
![image](https://github.com/gunjankhanal/assessmentk8s/assets/20742236/ac4f45fd-73b0-46c9-86da-68072399ad2a)
![image](https://github.com/gunjankhanal/assessmentk8s/assets/20742236/9a17abdf-32a7-4a8f-adab-a0c3870c476e)
![image](https://github.com/gunjankhanal/assessmentk8s/assets/20742236/58111515-329e-4a66-8840-93fde1aaeda5)
![image](https://github.com/gunjankhanal/assessmentk8s/assets/20742236/862a2491-04bb-449b-857c-eef81fb6adcb)
![image](https://github.com/gunjankhanal/assessmentk8s/assets/20742236/f2a0ed1b-59c0-45ef-a544-de1bedb3e4fa)

 
 
 
 

 
  

  


