## PhpCodeAnalyzer Docker Container.
[![Docker Pulls](https://img.shields.io/docker/pulls/rvannauker/phpca.svg)](https://hub.docker.com/r/rvannauker/phpca/) [![Docker Stars](https://img.shields.io/docker/stars/rvannauker/phpca.svg)](https://hub.docker.com/r/rvannauker/phpca/) [![](https://images.microbadger.com/badges/image/rvannauker/phpca:latest.svg)](https://microbadger.com/images/rvannauker/phpca:latest) [![GitHub issues](https://img.shields.io/github/issues/RichVRed/docker-phpca.svg)](https://github.com/RichVRed/docker-phpca) [![license](https://img.shields.io/github/license/RichVRed/docker-phpca.svg)](https://tldrlegal.com/license/mit-license)

Docker container to install and run phpca

### Installation / Usage
1. Install the rvannauker/phpca container:
```bash
docker pull rvannauker/phpca
```
2. Run phpca through the phpca container:
```bash
sudo docker run --rm --volume $(pwd):/workspace --name="phpca" "rvannauker/phpca" --no-progress {destination}
```

### Download the source:
To run, test and develop the PHPUnit Dockerfile itself, you must use the source directly:
1. Download the source:
```bash
git clone https://github.com/RichVRed/docker-phpca.git
```
2. Build the container:
```bash
sudo docker build --force-rm --tag "rvannauker/phpca" --file phpca.dockerfile .
```
3. Test running the container:
```bash
 $ docker run rvannauker/phpca --help
```