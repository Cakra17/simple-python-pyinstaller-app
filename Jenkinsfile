node {
    agent none
    stage('Build'){
        try{
            docker.image('python:2-alpine').inside {
                sh 'python -m py_compile sources/add2vals.py sources/calc.py'
            }
        } catch (e) {
            throw e
        }
    }
}