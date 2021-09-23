# seircast-html
SEIRcast.org static html files

### how to build/run
1. docker build -t dockerstaticweb .
2. docker run -p 80:80 dockerstaticweb

### how to push to azurecr
1. docker login seircastusf.azurecr.io -u seircastusf (need to create/enable access key in Azure portal.)
2. docker tag dockerstaticweb seircastusf.azurecr.io/dockerstaticweb
3. docker push seircastusf.azurecr.io/dockerstaticweb
