# oauth2-server
基于spring boot2 sso Oauth2 Server服务

#创建API数据库
CREATE DATABASE IF NOT EXISTS oauth2_server DEFAULT CHARSET utf8 COLLATE utf8_general_ci;
grant all privileges on oauth2_server.* to oauth2_server@localhost identified by 'password_dev';

#可以支持的授权模式：implicit,authorization_code,refresh_token,password,client_credentials
# http://localhost:8080/oauth/token?grant_type=password&scope=read&client_id=SampleClientId&client_secret=secret&username=zhangsan&password=password

#token公钥地址,用于本地验证token
#http://localhost:8080/oauth/token_key

#验证token地址
#http://localhost:8080/oauth/check_token?token=XXXXXX
