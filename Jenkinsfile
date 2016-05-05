#!groovy    

/**
 * 
 * - One of the easiest ways to get a clean build is to use a container 
 * - The image is fetched, if one is not already available on the worker * 
 * 
 */ 
 
inContainer {
    
    /** 
     * - specify any docker image
     */
    image "cloudbees/tools"
    
    /**
     * 
     * - The build script can call a script in your project, or your favourite build tool
     * 
     */ 
    build_script = "./bin/ci"
    
    /**
     * 
     * - Optionally, tests can be run as a separate stage. 
     * - Test results, if they are in the junit/xunit format, can be collected
     * - When there are failing tests detected, the build is marked as unstable
     */ 
    test_script = "./bin/ci_test"
    testResults = "/tests"
    
    
    /** 
     * - Notify your team of the good, or bad news.  
     */
    slack = "#engineering"
    
}       




        
    
