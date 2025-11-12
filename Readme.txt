docker rm -f nginx-react-struts-totaldocs-login-front

docker run --name nginx-react-struts-totaldocs-login-front ^
-v "%cd%\frontend\dist:/usr/share/nginx/html" ^
-v "%cd%\nginx.conf:/etc/nginx/nginx.conf" ^
-p 80:80 -d nginx
