# Docker jenkins


## Documentation

	git clone https://github.com/raonis/jenkins.git

Pull docker Jenkins:

	docker pull jenkins/jenkins:lts


# Fisrt step ( Basic instrutions )

	docker run -p 8080:8080 -p 50000:50000 -v jenkins_home:restore/jenkins_home jenkins/jenkins:lts

For backup jenkins:

	CONTAINER=`docker ps | grep jenkins | awk '{print $1}'`
	docker cp $CONTAINER:/var/jenkins_home 

