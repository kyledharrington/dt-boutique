## Hello! This repo has been forked from the google mircroservices boutique app.

Deploying this yaml will create a version of the Google mircroservices boutique app with a couple of modfications:
- added an nginx front end service and pods
- added a config map to allow for dynatrace log collection

# Getting started
1. Create a Kubernetes cluster (any flavor, your choice)
1. Create a local copy of this repo in a spot where you can connect to K8s via `kubectl` (e.g. from a cloud shell):
   1.  `git clone https://github.com/kyledharrington/dt-boutique.git`
1. Create the resources:
   1. `kubectl apply -f dt-boutique/dt-boutique.yaml`
1. Confirm resources were created:
   1. `kubectl get all`  
