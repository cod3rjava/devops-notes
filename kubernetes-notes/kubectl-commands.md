{\rtf1\ansi\ansicpg1252\cocoartf2761
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;}
{\*\expandedcolortbl;;}
\paperw11900\paperh16840\margl1440\margr1440\vieww11520\viewh8400\viewkind0
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0

\f0\fs24 \cf0 # Kubernetes Resources\
\
---\
\
# Official Documentation\
\
* https://kubernetes.io/docs/home/\
* https://kubernetes.io/docs/reference/kubectl/quick-reference/\
\
---\
\
# Kubectl Commands\
\
# Pod Creation\
\
* `kubectl run nginx --image=nginx` # Create a pod named nginx with the nginx image.\
\
# Deployment and Service Creation\
\
* `kubectl create deploy nginx-deploy --image=nginx` # Create a deployment named nginx-deploy with the nginx image.\
* `kubectl expose deploy nginx-deploy --port=80` # Expose the nginx-deploy deployment on port 80.\
\
# Describing Resources\
\
* `kubectl describe resourcetype resource name` # General command to describe a resource.\
* `kubectl describe pod nginx` # Describe the pod named nginx.\
\
# Viewing Logs\
\
* `kubectl logs nginx` # View logs for the pod named nginx.\
\
# Getting Resources\
\
* `kubectl get pods` # List all pods.\
* `kubectl get deploy` # List all deployments.\
* `kubectl get svc` # List all services.\
* `kubectl get ep` # List all endpoints.\
\
# Editing Resources\
\
* `kubectl edit deploy deployname` # Edit a deployment by name.\
\
# Rollout Management\
\
* `kubectl rollout status` # Check the status of a rollout.\
* `kubectl rollout restart deployname` # Restart a deployment.\
* `kubectl rollout undo deployname` # Undo the last rollout of a deployment.\
\
# Applying Configuration Files\
\
* `kubectl create -f filename` # Create resources from a file.\
* `kubectl apply -f filename` # Apply changes to resources from a file.}