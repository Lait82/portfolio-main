create ssl folder in main directory
‘‘‘
mkdir -p webserver/ssl

openssl req -x509 -nodes -days 365 -newkey rsa:2048 \
 -keyout webserver/ssl/localhost.key \
 -out webserver/ssl/localhost.crt \
 -subj "/CN=localhost"
‘‘‘
