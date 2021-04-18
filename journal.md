request-timer AB testing
------------------------

Launch the test from jumphost:
1. Pre-req:
    ```
    ulimit -n 20000
    oc scale --replicas=40 deploymentconfig request-timer
    ```
2. Then, launch the test:
    ```
    ab -k -n 300000 -c 1500 https://request-timer-load-testing.appls.labcert01.dev.boa.paas.cloudcenter.corp/request-timer/v1/api/timer/fixed/100
    ```