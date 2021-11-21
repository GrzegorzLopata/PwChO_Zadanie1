# PwChO_Zadanie1

Zadanie 1
Podpunkt 3)
a) docker build . -t nazwa/node-web-app
b) docker run -p 49160:8080 -d nazwa/node-web-app
c) docker exec -it 470579555dba /bin/bash
d) docker image inspect nazwa/node-web-app | jq '.[].RootFS'

Datę można wyświelić za pomocą polecenia:
  curl -i localhost:49160

Efekt powyższego polecenia:
    HTTP/1.1 200 OK
    X-Powered-By: Express
    Content-Type: text/html; charset=utf-8
    Content-Length: 11
    ETag: W/"b-Ck1VqNd45QIvq3AZd8XYQLvEhtA"
    Date: Sun, 21 Nov 2021 20:53:48 GMT
    Connection: keep-alive
    Keep-Alive: timeout=5
    
Podpunkt 4)
Obraz można zbudować używając komendy docker build <link do repozytorium>:
- docker build -t user/repo:tag
- docker push user/repo:tag
