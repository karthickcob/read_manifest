pipeline {
	agent {
		label "Karthick"
	}
	
stages {
		stage('Read manifest') {
			steps {
				script {
					def connStrings = new XmlSlurper().parseText("manifest.xml")
                    println "Environment name : ${connStrings.manifest.testSuiteName}"
                    println "Connection name : ${connStrings.manifest.robotFrameworkDir}"					
				}
			}
	}	
}
        }
