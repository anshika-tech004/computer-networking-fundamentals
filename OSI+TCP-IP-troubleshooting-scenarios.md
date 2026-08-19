## Scenario 1 : No Internet- ethernet cable disconnected
- SYMPTOM:
   - computer is showing no network connection
- OSI Model:
    - Layer1 (Physical layer)
- TCP/IP Model:
     - Layer1 (Network access layer)
- POSSIBLE CAUSE:
     - Cable disconnected
     - Damaged cable
     - Router/switch port problem
- Troubleshooting:
     - Check the cable
     - Check network adapter
     - try another cable or router port
> What I learned
   - I learned that having a wifi connection does not always means that the laptop has internet access there might be
     possible causes like damaged cable, router problem etc..

## Scenario 2 : Connected to network but cannot communicate with a LAN device
- SYMPTOM:
    - laptop is connected to local network but it cannot communicate with another device on the same LAN like printer
- OSI LAYER:
    - Layer2 (Data Link Layer)
- TCP/IP LAYER:
    - Layer1 (Network Access Layer)
- POSSIBLE CAUSE:
    - Wrong VLAN
    - MAC related problem
    - Switch config. issue
- TROUBLESHOOTING
    - Check VLAN config.
    - Local firewall blocking communication
    - Test connectivity
> What I learned
   - I learned that being connected to same network does not automatically guarantee communication between LAN devices.

## Scenario 3 : Wrong IP address
- SYMPTOM:
    - laptop is connected to network but it receives incorrect IP config.
- OSI LAYER:
    - Layer 3 (Network layer)
- TCP/IP LAYER:
    - layer2 (Internet layer)
- POSSIBLE CAUSE:
    - Incorrect IP address
    - Incorrect IP config.
- TROUBLESHOOTING
     - Check whether the IP address is valid
     - check IP config.
> What I learned
   - I learnt that incorrect IP address can prevent a laptop from communicating with local or external networks

## Scenario 4 : TCP port is blocked
- SYMPTOM:
   - laptop can reach a server but a particular service on the server is not accessible.
- OSI LAYER:
   - Layer 4(Transport layer)
- TCP/IP LAYER:
    - Layer3 (Transport layer)
- POSSIBLE CAUSE:
    - Firewall blocking port
    - Incorrect port
- TROUBLESHOOTING:
    - Check firewall rules
    - test specific TCP port
    - check basic IP connectivity
> What I learned
   - I learnt that successful IP connectivity does not necessarily mean particular application service is accessible.
   - TCP ports allow specific service to communicate

# Scenario 5 : Session keeps disconnecting
- SYMPTOM:
    - a remote session with a server was established but the connection keeps dropping after a short period.
- OSI LAYER:
    - Layer 5 (Session layer)
- TCP/IP LAYER:
    - Layer 4 (Application layer)
- POSSIBLE CAUSE:
    - Session timeout
    - session expiration
    - unstable network connection
- TROUBLESHOOTING:
    - Check session timeout setting
    - try establishing a new session
    - check the network connection
> What I learned
   - I learnt that a session is responsible for maintaining and managing the ongoing interaction.
   - Session can disconnect even though you have a proper network connection.


## My understanding
  - These scenarios helped me understand how OSI and TCP/IP models can be used as practical troubleshooting frameworks
    rather than just theoretical models.
