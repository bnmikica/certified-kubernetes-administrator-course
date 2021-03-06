# Practice Test - Namespaces
  - Take me to [Practice Test](https://kodekloud.com/courses/539883/lectures/9816576)

Solutions to practice test for namespaces

1. Run the command **`kubectl get namespace`** and count the number of pods.
   
   <details>

   ```
   $ kubectl get namespace
   $ kubectl get ns --no-headers | wc -l
   ```
   </details>

1. Run the command **`kubectl get pods --namespace=research`**
   
   <details>

   ```
   $ kubectl get pods --namespace=research
   $ kubectl get pods -n research --no-headers | wc -l
   ```
   </details>

1. Run the below command

   <details>

   ```
   $ kubectl run redis --image=redis --namespace=finance
   $ kubectl run redis --image=redis --dry-run=client -o yaml > pod.yaml
   ```
   </details>

1. Run the command **`kubectl get pods --all-namespaces`**

   <details>

   ```
   $ kubectl get pods --all-namespaces
   $ kubectl get pods --all-namespaces | grep blue
   ```
   </details>

1. Connectivity Test
   
   <details>

   ```
   Host Name: db-service and Host Port: 3306
   ```
   </details>

1. Connectivity Test

   <details>

   ```
   $ kubectl get svc -n dev 
   Host Name: db-service.dev.svc.cluster.local and Host Port: 3306
   ```
   </details>


#### Take me to [Practice Test Solutions](https://kodekloud.com/courses/539883/lectures/16416900)
