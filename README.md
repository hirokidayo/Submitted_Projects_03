# AWSの設定
以下コマンドで、アクセスキー、シークレットキー、リージョン、フォーマットを設定する
```bash
aws configure
```
設定内容を確認する
```bash
aws configure list
```

# サービスをEKSへデプロイ
```bash
aws eks --region us-east-1 update-kubeconfig --name demo
kubectl cluster-info
kubectl apply -f database.yaml
kubectl get pods
kubectl get services
 
kubectl get svc
kubectl get pods
kubectl describe svc <DATABASE_SERVICE_NAME>
kubectl get deployments
kubectl describe deployment <SERVICE_NAME>
```