# kubernetes の 学習用リポジトリ

## 概要

* dojo / [Kubernetes道場](https://cstoku.dev/posts/2018/k8sdojo-01/)を使って学習する
* sample_service / 簡単なサービスをk8sで構築する

## 環境構築

### Kubernetesインストール
* [参考](https://kubernetes.io/ja/docs/tasks/tools/install-kubectl/#macos%E3%81%B8kubectl%E3%82%92%E3%82%A4%E3%83%B3%E3%82%B9%E3%83%88%E3%83%BC%E3%83%AB%E3%81%99%E3%82%8B)

```shell

# インストール
curl -LO https://storage.googleapis.com/kubernetes-release/release/$(curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt)/bin/darwin/amd64/kubectl

# パーミッション変更
chmod +x ./kubectl

# パスを通す
sudo mv ./kubectl /usr/local/bin/kubectl

# 確認
kubectl version
```

### Minikube

* [参考](https://minikube.sigs.k8s.io/docs/start/macos/)

```shell

# インストール & パスを通す
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-darwin-amd64 \
  && sudo install minikube-darwin-amd64 /usr/local/bin/minikube

# スタート
minikube start

# ストップ
minikube stop
```
