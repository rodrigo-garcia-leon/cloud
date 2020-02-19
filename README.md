# cloud

Collection of scripts to manage Google Cloud Platform and Kubernetes ☁️

## install

```sh
brew cask install google-cloud-sdk
```

## setup

```sh
gcloud init
gcloud config set compute/zone europe-west1
gcloud container clusters create cloud --num-nodes=1
gcloud container clusters get-credentials cloud
```

## usage

```sh
kubectl diff -f configs/
kubectl apply -f configs/
```
