pipeline {
    agent any

    parameters {
        booleanParam(defaultValue: false, description: "Enable Service?", name: "myBoolean")
    }

    stages  {
        stage("Demo") {
            steps {
                echo "booleanParams is set to: ${params.myBoolean}"  
            }
        }
    }
}