pipeline{
agent any
tools{
gradle 'Gradle'
jdk 'JDK'
}
stages{
stage('Checkout'){
steps{
git branch:'master',url:'https://github.com/varshini663/FinGrad.git'
}
}
stage('Build'){
steps{
sh 'gradle build'
}
}
stage('Run'){
steps{
sh 'gradle test'
}
}
stage('run'){
steps{
sh 'gradle run'
}
}
}
post{
success{
echo 'successful'
}
failure{
echo 'not'
}
}
}
