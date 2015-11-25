# Dockerfile-openssl-gost

### Usage

    docker run --rm -i -t -v `pwd`/keys:/keys dmitryromanov85/openssl-gost openssl req -engine gost -newkey gost2001 -pkeyopt paramset:A -x509 -extensions v3_ca -passout pass:135246 -subj "/C=RU/ST=Moscow/L=Moscow/O=organization/CN=sample.ru/emailAddress=user@sample.ru" -keyout priv.pem -out req.csr

Your key and certificate in folder keys
