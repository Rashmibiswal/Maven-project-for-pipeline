pipeline
{
    agent any
    stages{
        stage('scm checkout')
        {
            steps{
               git branch: 'master', url: 'https://github.com/renuashu/Maven-project-for-pipeline'
                }
        }
        stage('please compile code')
        { 
            steps { withMaven(globalMavenSettingsConfig: '--- Use system default settings or file path ---', jdk: 'JDK_HOME', maven: 'MVN_HOME', mavenSettingsConfig: '--- Use system default settings or file path ---') 
                 {sh 'maven compile'}
   
}

}

        }





    }
