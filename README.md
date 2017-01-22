# stackoverflow-41747843
Demo for Stackoverflow Question http://stackoverflow.com/questions/41747843/pass-environment-variables-from-docker-compose-to-container-at-build-stage

With docker-compose 
===================
`docker-compose build`
`docker-compose up`

With docker build & run
===================
docker build . --no-cache -t stackoverflow/env-test --build-arg REQUIREMENTS=requirements_dev.txt
docker run stackoverflow/env-test cat /usr/src/app/requirements_dev.txt
