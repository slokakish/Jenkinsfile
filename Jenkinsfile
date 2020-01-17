node {
def mvnhome
stage("checkout")
{
git 'https://github.com/slokakish/hello-world-war.git'
}
mvnhome = tool 'MAVEN_HOME'
stage ("compilation")
{
sh "'${mvnhome}/bin/mvn' compile"
}
stage ("packaging")
{
sh "'${mvnhome}/bin/mvn' package"
}
stage ("result")
{
echo "successfull"
}
}
