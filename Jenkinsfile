def secret = 'Ebook'
def server = 'sgnd@192.168.3.174'
def directory = 'production/ebook/fullstack/stage1/chapter2/FS-S1-CP2-Introduction'
def branch = 'Deploy'
def image = 'registry.mejik.xyz/ebook/fs-s1-cp2-introduction'
    
pipeline{
    agent any
    stages{
        stage ('git pull'){
            steps{
                sshagent([secret]) {
                    sh """ssh -o StrictHostKeyChecking=no ${server} << EOF
                    cd ${directory}
                    git checkout .
                    git pull origin ${branch}
                    docker system prune -f
                    exit
                    EOF"""
                }
            }
        }
        stage ('build and push to registry'){
            steps{
                sshagent([secret]) {
                    sh """ssh -o StrictHostKeyChecking=no ${server} << EOF
                    cd ${directory}
                    docker-compose build
                    docker push ${image}
                    exit
                    EOF"""
                }
            }
        }
        stage ('redeploy'){
            steps{
                sshagent([secret]) {
                    sh """ssh -o StrictHostKeyChecking=no ${server} << EOF
                    cd ${directory}
                    sh redeploy.sh
                    docker rmi ${image}
                    exit
                    EOF"""
                }
            }
        }
    }
}
