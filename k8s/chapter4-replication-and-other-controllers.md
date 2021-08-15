### Liveness probes

Checks if the container is alive.

> But for a better liveness check, you’d configure the probe to perform requests on a specific URL path (/health, for example) and have the app perform an internal status check of all the vital components running inside the app to ensure none of them has died or is unresponsive.
> Be sure to check only the internals of the app. For example, the probe should not fail if the server cannot connect to the database. Restarting won't help in that case.


