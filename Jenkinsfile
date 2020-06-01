node {
checkout scm
def customImage = docker.build("my-image:${env.BUILD_ID}")
customImage.inside {
bat label: '', script: 'make test'
}
}
