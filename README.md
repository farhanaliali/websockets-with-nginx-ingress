# Node.js WebSocket example in kubernetes

This is a small demo which demonstrates the use of WebSocket in kubernetes.

## Steps

These are the steps to be executed in order to start the demo.

### Build the image

    docker build -t farhanluckali/websocket-demo .

### Push image to repo 

    docker push farhanluckali/websocket-demo

### deploy image to kubernetes 

    kubectl create -f deployment.yaml

### expose via ingress  

    kubectl create -f ingress.yaml


### testing 

    ws://{ingress-url}


