# vts-spring-config-server

This project was created to demonstrate the problem documented in <https://github.com/spring-cloud/spring-cloud-config/issues/1480>

1. Run the class VTSConfigServerApplication.
2. Go to <http://localhost:8888/SomeApplication1/dev/master> (through Postman, or browser, etc.)
Note: As expected, there are no errors in the log at this point because the only uri in the bootstrap file that is matched is the default uri.
3. Go to <http://localhost:8888/webapp/dev/master>.
Expected: No error is logged.
Observed: There are errors in the log: "More than one git repo URL template matched URL".
