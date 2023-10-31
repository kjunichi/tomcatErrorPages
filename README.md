# What is this

tomcatでウェブアプリ全体のエラーページを設定するにはどうしたら良いのかを学習した。
webapps/ROOT配下にエラーページを置き、conf/web.xmlにHTTPコード別にページを指定すれば良い
ことが分かった。

# How to use

```
 docker run -it --rm -p 8888:8080 -v `pwd`/webapps:/usr/local/tomcat/webapps -v `pwd`/conf:/usr/local/tomcat/conf tomcat:9.0
```

