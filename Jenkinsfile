node('node') {


    currentBuild.result = "SUCCESS"

    try {

       stage 'Checkout'

            checkout scm

       stage 'Test'

            env.NODE_ENV = "test"
            print "Environment will be : ${env.NODE_ENV}"
            echo 'test'
        
       stage 'Build'

            echo 'build'

       stage 'Deploy'

            echo 'build'

        }


    catch (err) {

        currentBuild.result = "FAILURE"

            echo 'error detected'

        throw err
    }

}
