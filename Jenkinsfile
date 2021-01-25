 node {
   
      stage('Git clone') {
        git credentialsId: 'git', url: 'https://git-codecommit.us-east-1.amazonaws.com/v1/repos/ks'
    }
       stage('clean') {
       sh 'mvn clean'
    }
       stage('compile') {
       sh 'mvn compile'
    }
	stage('test') {
        sh 'mvn test'
    }
	stage('package') {
        sh 'mvn package'
    }
	stage('deploy') {
        sh 'mvn deploy'
    }
}
