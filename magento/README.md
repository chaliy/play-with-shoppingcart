# Run

    docker-compose up -d # Will not work unfortunatelly
    
# Source
    docker run --name mariadb -td -e USER=user -e PASS=password paintedfox/mariadb
    docker run --name memcached -d -p 11211 sylvainlasnier/memcached
    docker run -td -p 80:80 --link mariadb:db --link memcached:cache paimpozhil/magento-docker

