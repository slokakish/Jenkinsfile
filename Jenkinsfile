node {
def mvnhome
stage("checkout")
{
git 'https://github.com/bheem25kyack/course.git'
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