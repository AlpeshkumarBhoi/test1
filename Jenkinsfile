node () {

	stage ('new maven build - Checkout') {
 	 checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '', url: 'https://github.com/AlpeshkumarBhoi/test1.git']]]) 
	}
	stage ('new maven build - Build') {
    sh """
			cd $WORKSPACE
			ls -lrta
			mvn install		
 			""" 
			} 
 		} 
	
