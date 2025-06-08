pipeline{
	agent any
	tools{
		gradle 'Gradle'
		jdk 'JDK'
	}
	stages{
		stage('Checkout'){
		step{
		 git branch:'master',url:'https://github.com/varun0981/varungrad.git'
			}
		}
		stage('Build'){
		step{
		sh'gradle run'
			}
		}
		stage('Test'){
		step{
		sh'gradle test'
			}
		}
		stage('Run Application'){
		step{
		sh'gradle run'
			}
		}
	}
}

