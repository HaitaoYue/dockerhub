FROM alpine/git

RUN cd /tmp && git clone https://github.com/HaitaoYue/dockerhub.git && \
	cd dockerhub && lastTag=$(git describe --tags `git rev-list --tags --max-count=1`) && \
	echo $lastTag && git checkout -b $lastTag $lastTag
