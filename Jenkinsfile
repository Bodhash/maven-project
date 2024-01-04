pipeline
{
    agent any
    stages
    {
        stage ('scm checkout')
        { steps { git branch: 'master', url 'https://github.com/Bodhash/maven-project' }}

        stage ('execute unit test framework')
        {steps {withMaven(globalMavenSettingsConfig: '86f85bab-965d-4d46-b5f2-68e630786596', jdk: 'LOCALJDK', maven: 'LOCALMVN', mavenSettingsConfig: '	3a5052be-00c2-42d4-82cb-2da182333691', traceability: true) 
        { sh 'mvn test'   //maven tset goal
         }
         }}

}
        
}
