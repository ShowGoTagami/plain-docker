# Docker入門

Docker入門として、以下ができるようになることを目指しています。

・development build
・production build
・run test

# 始め方

## developmentで動かす

```
$ docker-compos up
```

`localhost:3000` へアクセス


localファイルを変更してもbuildが走るので変更が反映される

## productionで動かす

```
$docker-build .

...
 ---> Using cache
 ---> 982b375abfa2
Successfully built 982b375abfa2
...

$ docker run -p 8080:80 982b375abfa2 <=IDをコピペ
```
