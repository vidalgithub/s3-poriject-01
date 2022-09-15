# s3-poriject-01
This is a k8s project. 
PROBLEM TO SOLVE
Deploy Espresso Shop microservice application on Kubernetes Cluster

Main goal  from the customer
Customer name: EXPRESSO INC
EXPRESSO INC business is growing exponentially at the extern that we  the headquarter has expressed the need to launch an online shop where millions of customers will be able to shop and post review on different coffer flavor they offer.
To satisfy that need and after a careful selection EXPRESSO INC have picked  EK TECH SOFTWARE SOLUTION as their  best IT firm to build a robust application that will meet  and exceed  their expectation.

Requirements from the customer
1-  High availability
2-  zero downtime
3-  Biweekly deployment
4-  On demand scalability

Requirement from Development teamShop-web
Expose  container on port 80
Set the following environment variables:
ProductCatalogUrl=http://espresso-shop-product-catalog-svc:8091
ReviewsUrl=http://espresso-shop-reviews-svc:8092
Use container image devopseasylearning2021/s3-project01-espresso-shop:v1.0.0 

Requirement from Development teamShop-product
Expose  container on port 80
Set the following environment variables:
Create label          version: v1
Use container image devopseasylearning2021/s3-project01-espresso-shop-product:v1.0.0 

Requirement from Development teamShop-review1
Expose  container on port 80
Set the following environment variables:
Create label          version: v1
Set the following environment variables:
    SERVICE_VERSION = v1
Use container image devopseasylearning2021/s3-project01-espresso-shop-review:v1.0.0 

Requirement from Development teamShop-review2
Expose  container on port 80
Set the following environment variables:
Create label          version: v2
Set the following environment variables:
    SERVICE_VERSION = v2
Use container image devopseasylearning2021/s3-project01-espresso-shop-review:v1.0.0 

DevOps team Brainstorm
Deployment strategy:  Kubernetes.
Deployment management helm chart.

DevOps team service overview
  Pod Name                      Port
  shop-product                  8091
  shop-reviews                  8092
  shop-web                      8090
  


  
  
 





