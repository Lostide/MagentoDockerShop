This rep was created using information provided in this article: https://www.magemodule.com/all-things-magento/magento-2-tutorials/docker-magento-2-development/
YouTube channel of this beautiful man, who wrote the article provided above: https://www.youtube.com/channel/UCNEzMoTx-F226jxiT0rY8dA

Useful commands:
1. To bash into app container, of course it depends on the name of a container:

docker exec -it web bash

2. Commands to use for magento 2 installation. Should edit the data:

    php bin/magento setup:install \
    --admin-firstname=John \
    --admin-lastname=Doe \
    --admin-email=johndoe@example.com \
    --admin-user=admin \
    --admin-password='SomePassword123' \
    --base-url=https://local.domain.com \
    --base-url-secure=https://local.domain.com \
    --backend-frontname=admin \
    --db-host=mysql \
    --db-name=magento \
    --db-user=root \
    --db-password=root \
    --use-rewrites=1 \
    --language=en_US \
    --currency=USD \
    --timezone=America/New_York \
    --use-secure-admin=1 \
    --admin-use-security-key=1 \
    --session-save=files \
    --use-sample-data
