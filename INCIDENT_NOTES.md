Manual Chaos Test
Objective
Test service failure and recovery procedures.

Service Tested
Apache Web Server (apache2)

Failure Simulation
The Apache service was intentionally stopped.

Command: sudo systemctl stop apache2

Result: Service became inactive and the web application was unavailable.

Recovery
The Apache service was restarted.

Command: sudo systemctl start apache2

Result: Service returned to active state and application accessibility was restored.

Verification
curl http://localhost

The application responded successfully after recovery.

Conclusion
Manual chaos testing successfully demonstrated service recovery capability.
