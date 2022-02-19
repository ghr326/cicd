# cicd
simple devops project
  continous integration
  contionous dellivery
  continous deployment
      continous integration:
          we have source code in our local work stations 
          from there we will commmit it into the version control systems
          once the code is available in the vcs the ci tool will automatically pull the code build the code and run the unit tests then we call it as a contionous integration
         
         
      continous deployment:   
         during this ci process we will build our source code or compile our source code and generate artifacts 
          once the artifacats are generated we need to deploy on target environments
          target environment may be changed it may be a dev test or qa  or prod
          take an example if we want to deploy artifacts in a staging environment we need to do the regression test and performance test 
          once it is passed we can deploy into the production environment
          
          we do the regression test and performance test
         
          
      
      continous delivery:
          where if we want to deploy the artifacts into the staging or production we need manager approval this manual type of deployment is called continous delivery
      
      
                                                        DEVOPS PROJECT:
                                                               
                                                             
                  (PULL CODE)                      (COPY ARTIFACTS)                 (DEPLOY CONAINER)
      GIT HUB------------------>JENKINS------------------------------------>ANSIBLE-------------------KUBERNETES
         ^                         |                                           \                         ^         
         |                         |                                             \                      /       
         | (COMMIT CHANGES)        |(BUILD CODE)                                   \                  /     
         |                         V                                (PULL IMAGE)     \              /    (PUSH IMAGE)
      GIT LOCAL OR CLIENT         MAVEN                                                V          /  
                                                                                       DOCKER  HUB     
      
      CONTINOUS INTEGRATION                                                        CONTINOUS DEPLOYMENT
      
      
      
      
      
      
      
                        
