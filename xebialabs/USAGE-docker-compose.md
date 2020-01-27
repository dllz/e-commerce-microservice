# XL DevOps Platform Usage

This blueprint allows you to run test instances in Docker of:

* XL Deploy
* XL Release
* Jenkins

## Configuration

Copy `xebialabs/config.yaml` to `$HOME/.xebialabs` or make sure your `$HOME/.xebialabs/config.yaml` contains:

```plain
xl-deploy:
  authmethod: http
  password: admin
  url: http://localhost:4516/
  username: admin
xl-release:
  authmethod: http
  password: admin
  url: http://localhost:5516/
  username: admin
```

## Start the containers

Run the following:

```plain
cd docker
docker-compose up [--detach]
```

> **Note:** If you omit `--detach`, Docker will take command of your terminal and you will need to open another to apply the blueprints.

## Find the apps here

* XL Deploy: http://localhost:4516
  * username: admin
  * password: admin

* XL Release: http://localhost:5516
  * username: admin
  * password: admin

* Jenkins: http://localhost:8080
  * username: admin
  * password: admin

## Notes

* You can obtain a trial license or bring your own license for the XL Platform.