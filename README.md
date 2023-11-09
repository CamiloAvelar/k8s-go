# k8s-go

## DEPLOYING
- k3d cluster create k8s-go -p 80:80
- cd deployment
- kubectl apply -k ./
- curl -v go.localdev.me/?name=Camilo

## BUILDING AND PUSHING
- go build
- docker build -t k8s-go .
- docker tag k8s-go camiloavelar/go-hello-world:X
- docker push camiloavelar/go-hello-world:X