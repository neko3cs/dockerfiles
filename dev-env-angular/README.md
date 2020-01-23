# dev-env-angular

Angular の開発環境。

## How to use

```
$ docker build -t dev-env-angular .
$ docker run -itd --hostname dev-env-angular --name dev-env-angular -p 8080:80 dev-env-angular bash
$ docker exec -it dev-env-angular bash
```
