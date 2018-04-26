
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
                
                sh 'gcovr -x -r . > OpenCppCoverageDemo/cmake/x64/debug/reports/gcovr_report.xml'

        }
}
