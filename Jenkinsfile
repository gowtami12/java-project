pipeline{
agent any
stages
{
stage('build')
{
steps{
sh 'ant -f build.xml -v'
}
}
}
post{
always{
archive '/var/lib/jenkins/workspace/My%20Java-project/dist/*.jar'
}
}
}
