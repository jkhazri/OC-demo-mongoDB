# OC-demo-mongoDB
This is a simple demo on how to deploy a MongoDB on K8s.
you need first to clone the project and move under the  OC-demo-mongoDB folder.
then run thos command : 
```bash
git clone https://github.com/jkhazri/OC-demo-mongoDB.git
cd OC-demo-mongoDB
```
1. Create a Persistent Volume (PV) and Persistent Volume Claim (PVC):
```bash
kubectl apply -f mongo-pv.yaml
```
2.Create a ConfigMap for MongoDB configuration:
```bash
kubectl apply -f mongo-configmap.yaml
```
3. Deploy MongoDB StatefulSet:
```bash
kubectl apply -f mongo-statefulset.yaml
```
4. Create a MongoDB Service:
```bash
kubectl apply -f mongo-service.yaml
```
