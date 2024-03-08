# Deploy http echo

Useful web application to display the request HTTP headers as well as other data depending of options passed in the request.
See [docker-http-https-echo](https://github.com/mendhak/docker-http-https-echo) for more details.

## Deployment to the test cluster
- Login to the test cluster
- Run kubectl: `kubectl apply -f manifests`

## Access app
- Access in a web browser: https://http-echo.test.teacherservices.cloud/
- Or via curl: `curl https://http-echo.test.teacherservices.cloud/`
- The application logs also show the data: `kubectl -n infra logs deployment/http-echo -f`

## Delete from the test cluster
- Login to the test cluster
- Run kubectl: `kubectl delete -f manifests`
