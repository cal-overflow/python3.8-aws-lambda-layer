# python3.8-opencv-aws-lambda-layer

OpenCV Python3.8 layer for use with AWS Lambda. A simplified (only for python3.8 and pre-built) version of [iandow/opencv_aws_lambda](https://github.com/iandow/opencv_aws_lambda).

View the docker image on [DockerHub](https://hub.docker.com/repository/docker/caloverflow/python3.8-opencv-aws-lambda-layer).

### Getting the image layer files
```bash
# Run the docker image & copy the needed layer zip
docker run -rm -v $(pwd):/data caloverflow/python3.8-opencv-aws-lambda-layer:<TAG_VERSION> cp /packages/cv2-python38.zip /dat
```
See the [dockerhub repository](https://hub.docker.com/repository/docker/caloverflow/python3.8-opencv-aws-lambda-layer) for all tags. Use `latest` if you do not need a specific version.

### Upload the layer to AWS
- [Via CLI](https://github.com/iandow/opencv_aws_lambda#preliminary-aws-cli-setup)
- [Via AWS Console](https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html#configuration-layers-create)
