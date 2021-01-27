pipeline{

agent any

tools{
maven 'Maven 3.6.3'
}

stages{
stage('build'){
steps{
echo 'compile sysfoo app'
sh 'mvn compile'
}
}

stage('test'){
steps{
echo 'test sysfoo app'
sh 'mvn clean test'
}
}
stage('package'){
steps{
echo 'package sysfoo app'
sh 'mvn package -DskipTests'
}
}
}

}
