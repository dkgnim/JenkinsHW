pipeline {
  agent {

    docker {
      image 'cofaone/jenkins_hw1:jenkinshw'
    }

  }

  stages {

    stage('Run docker') {
      steps {
      sh 'docker login -v /var/run/docker.sock:/var/run/docker.sock-u cofaone -p 1qaz2wsx3edc'
      sh 'sudo docker pull -v /var/run/docker.sock:/var/run/docker.sock cofaone/jenkins_hw1:jenkinshw'
      sh 'sudo docker run -ti -v /var/run/docker.sock:/var/run/docker.sock dockercofaone/jenkins_hw1:jenkinshw'
            }
    }
  }
}