# cloud

Collection of scripts to manage Google Cloud Platform and Kubernetes ☁️

## install

```sh
brew cask install google-cloud-sdk
```

## setup

```sh
gcloud init
gcloud config set compute/zone europe-west1-b
gcloud container clusters create cloud --num-nodes=1
gcloud container clusters get-credentials cloud
gcloud compute addresses create cloud --global
```

## usage

```sh
kubectl diff -f configs/
kubectl apply -f configs/
```
