
node() {


        checkout scm


        stage("Package & Code Analysis") {
		sh 'chmod u+x ./build.sh'
		sh './build.sh'

        }
        stage("Sonar  Scan"){
              sh 'sonar-scanner'
        }
}
