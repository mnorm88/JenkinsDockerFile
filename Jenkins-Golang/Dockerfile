
FROM jenkins/jenkins:lts
# if we want to install via apt
USER root
RUN apt update && apt install -y golang-go
ENV GOPATH=/home/jenkins/workspace/slack-notification-test
RUN go get -u github.com/slack-go/slack
# drop back to the regular jenkins user - good practice
USER jenkins
