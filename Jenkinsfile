
node() {

        checkout scm

        stage("Build x64 Debug") {
		sh 'chmod u+x ./build.sh'
		sh './build.sh'
        }
        stage("Perform Unit Tests"){
                dir('OpenCppCoverageDemo/cmake/x64/debug'){
                   sh 'make TestSource_coverage'
                }
        }
}
