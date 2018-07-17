Build:
docker build -t oc-cli:3.7.0 .
usage:
docker run -it --add-host openshift-test.test.com:172.789.789.789  oc37  /bin/sh -c "oc login -u aaaaaa -p xxxxxx --insecure-skip-tls-verify openshift-test.test.com && oc project myproj-sit && oc get dc,pods,bc,is,svc"