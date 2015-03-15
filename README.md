# Mule Webapp Sample

This example demonstrates how to wrap a Mule application as a JavaEE web-application (WAR).

It exists to address the following common issues:

- Using HTTP instead of Servlet inbound endpoints,
  which works but makes no sense because it bypasses the web tier from the web container
  and starts a Mule HTTP server in it.
- Trying to deploy Mule as a Tomcat service
  (per [this guide](www.mulesoft.org/documentation/display/current/Deploying+Mule+as+a+Service+to+Tomcat)),
  which is complex, does not bring tons of benefits as opposed to simply deploying a WAR.

## Running the demo

    mvn jetty:run

You can then browse http://localhost:8889/mule-war-demo

**Copyright © 2015 David Dossot - MIT License**
