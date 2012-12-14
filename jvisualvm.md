# jvisualvm

To run : `jvisualvm`

To enable profiling in a remote server via jstat :

go to $JAVA_HOME/bin and create a file called `jstatd.all.policy` and paste these in :

    grant codebase "file:${java.home}/../lib/tools.jar" {
    permission java.security.AllPermission;};
   
Then start jstatd from the command line with :
    
    nohup jstatd -J-Djava.security.policy=jstatd.all.policy > jstatd.out 2>jstatd.err &


