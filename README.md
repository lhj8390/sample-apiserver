# sample-apiserver

API Aggregation 을 사용하여 sample api server 구현 <br/>
참고 라이브러리 : https://github.com/kubernetes/sample-apiserver

## code-generator 실행 방법

1. clone code-generator
    ```shell
    git clone https://github.com/kubernetes/code-generator
    ```
2. generate-groups.sh 실행

    ※ GOPATH 하위에서 실행 필요
    ```shell
   $GOPATH/src/k8s.io/code-generator/generate-groups.sh all \ 
      sample-apiserver/pkg/client sample-apiserver/pkg/apis "foo:v1" -h hack/boilerplate.go.txt  -o ../
   ```

