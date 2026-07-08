# Investigating PCAPs

## Objective


Reviewing and investing a suspicious PCAP from the client "BlueTeamLabs.online". Using WireShark and urldecoder to answer the scenario from blue team labs.  

### Skills Learned

- PCAP (Packet Capture) investigation.
- Security Operations Center (SOC) workflows.
- Malware traffic identification.
- Cyber threat hunting fundamentals.
- Wireshark navigation and filtering.
### Tools Used

- Wireshark.
- urldecoder.online.
- PCAP files.
## Steps
<img width="1018" height="848" alt="Extracting the file for the BlueTeamLabs scenario lab" src="https://github.com/user-attachments/assets/c2065289-dcc5-401f-94ec-d39137872a22" />

Ref 1: Extracting the file for the BlueTeamLabs scenario lab.

<img width="1012" height="850" alt="Checking stimetamp to verify with client" src="https://github.com/user-attachments/assets/7e497355-7bad-448f-9666-6a0de42540dc" />

Ref 2: Checking time stamp to verify with client.

<img width="1017" height="842" alt="Many protocols used, seeing exchanges of pcap" src="https://github.com/user-attachments/assets/38ceed5e-80c8-4c37-96ec-e0687c351f38" />

Ref 3: Many protocols used, seeing exchanges of pcap.

<img width="1021" height="554" alt="many packets sent from  4 to  5 and  5 to  2" src="https://github.com/user-attachments/assets/868def23-693d-4511-ab14-c0cd8ad45597" />

Ref 4: Many packets sent from  .4 to .5 and .5 to .2.

<img width="1017" height="558" alt="Source Port 41675 showing many times indicating a scan  Ports should should be unique per conneciton attempt" src="https://github.com/user-attachments/assets/e3ed3ddd-91cc-430e-b7c6-8d12ac2e411f" />

Ref 5: Source Port 41675 showing many times indicating a scan  Ports should should be unique per conneciton attempt.

<img width="777" height="445" alt="Port 80 and 22 are open on 10 251 96 5, since the bytes are different then the rest of the ports" src="https://github.com/user-attachments/assets/5e061e31-eb99-49cb-a7d4-0e4a54923218" />

Ref 6: Port 80 and 22 are open on 10.251.96.5, since the bytes are different then the rest of the ports.

<img width="792" height="333" alt="address  5 is communicating through port 80 which may indicate that it is a webserver, but we need verification" src="https://github.com/user-attachments/assets/b7f6d2fa-f5b8-4c8e-9d57-4cc3ec8debf3" />

Ref 7: Address .5 is communicating through port 80 which may indicate that it is a webserver, but we need verification.

<img width="1016" height="667" alt="Following the TCP stream on the HTTP protocol I have selected" src="https://github.com/user-attachments/assets/3a6a9ebe-2dfb-4380-ab73-48a347f6ce74" />

Ref 8: Following the TCP stream on the HTTP protocol I have selected.

<img width="744" height="720" alt="Showing conversation between client and server" src="https://github.com/user-attachments/assets/699ca938-555b-4612-bcde-983156be57c5" />

Ref 9: Showing conversation between client and server.

<img width="750" height="728" alt="Following the packet on HTTP stream and can read the traffick  Address 172 20 10 2 is coming from UBUNTU server" src="https://github.com/user-attachments/assets/648ff892-5992-4275-963d-5407ab74f074" />

Ref 10: Following the packet on HTTP stream and can read the traffick  Address 172.20.10.2 is coming from UBUNTU server.

<img width="972" height="283" alt="Packet 38 has a login" src="https://github.com/user-attachments/assets/82545714-d0fe-42da-8f65-4a45ad568e14" />

Ref 11: Packet 38 has a login.

<img width="746" height="700" alt="Stream shows username and password that was used for this login" src="https://github.com/user-attachments/assets/fb5dc7bc-e7cc-43e7-998e-4f5385b0c655" />

Ref 12: Stream shows username and password that was used for this login.

<img width="1014" height="840" alt="The beggining of trafick" src="https://github.com/user-attachments/assets/7bdfa558-a89b-4956-bbcf-c22ff43264aa" />

Ref 13: The beggining of traffic.

<img width="1019" height="786" alt="In scan we see many resets, but we see a SYN ACK on port 80" src="https://github.com/user-attachments/assets/86e74088-651e-430b-9373-803e85773661" />

Ref 14: In scan we see many resets, but we see a SYN ACK on port 80.

<img width="970" height="50" alt="Another SYN ACK with port 22" src="https://github.com/user-attachments/assets/53046637-9c2a-43ca-a731-4284ac849aac" />

Ref 15: Another SYN ACK with port 22.

<img width="1025" height="854" alt="Scan ends on packet 2166, the scan did not even take a second" src="https://github.com/user-attachments/assets/2ba11422-3486-4c8d-b81e-c6f9844ffaab" />

Ref 16: Scan ends on packet 2166, the scan did not even take a second.

<img width="962" height="15" alt="First communication from  4 to  5 on port 80" src="https://github.com/user-attachments/assets/f93ab146-e1a8-4433-8495-d172bdb5e408" />

Ref 17: First communication from .4 to .5 on port 80.

<img width="747" height="711" alt="same ubunto traffic, user agent is mozilla" src="https://github.com/user-attachments/assets/4c6c8e94-96ee-44de-9bd7-6caf67d385c7" />

Ref 18: Same ubunto traffic, user agent is mozilla.

<img width="1017" height="728" alt="packet 2215 has gobuster 3 0 1  Gobuster is a tool that can crawl directories" src="https://github.com/user-attachments/assets/efbc15ee-521d-425e-b5b8-7a60d5f42187" />

Ref 19: Packet 2215 has gobuster version 3.0.1. Gobuster is a tool that can crawl directories.

<img width="1019" height="719" alt="looking for success, searched HTTP1 1 200" src="https://github.com/user-attachments/assets/7b60cd08-0303-4460-8a44-bc52a0b98663" />

Ref 20: Looking for success, searched HTTP1 1 200.

<img width="1018" height="694" alt="made filter to find 200 on ip  5" src="https://github.com/user-attachments/assets/7a64cbaa-44ae-47c4-acb3-d1e7e7975ab1" />

Ref 21: Made filter to find 200 on ip .5.

<img width="1003" height="254" alt="Looking at length, big numbers indicate that the server has responded with something large" src="https://github.com/user-attachments/assets/2a05e90e-4d9d-4206-98f1-a41db531b593" />

Ref 22: Looking at length, big numbers indicate that the server has responded with something large.

<img width="732" height="674" alt="the begining of the response" src="https://github.com/user-attachments/assets/5d22cad9-4426-4d2c-bbc5-29e57a0f1f9f" />

Ref 23: The begining of the response.

<img width="731" height="680" alt="version of php showing, an attacker can look for an exploit and try to exploit this version" src="https://github.com/user-attachments/assets/3cca91df-2d45-4500-b79b-246f7bac3773" />

Ref 24: Version of php showing, an attacker can look for an exploit and try to exploit this version.

<img width="736" height="682" alt="Next big packet has mozilla, which can mean someone manually visited this directory" src="https://github.com/user-attachments/assets/7bc408ce-7f6e-4b74-a980-12f2a8138a3d" />

Ref 25: Next big packet has mozilla, which can mean someone manually visited this directory.

<img width="1018" height="663" alt="GET request by Gobuster was on packet 13661 and finished around 16 34 06" src="https://github.com/user-attachments/assets/8a9eeb2b-b416-4106-8bbb-ff948a8976d9" />

Ref 26: GET request by Gobuster was on packet 13661 and finished around 16:34:06.

<img width="970" height="17" alt="Spotted an upload package" src="https://github.com/user-attachments/assets/9955aede-d49b-40ff-a96c-9311f3ff637f" />

Ref 27: Spotted an upload package.

<img width="959" height="15" alt="13979 packet is a POST packet" src="https://github.com/user-attachments/assets/0db5296f-217b-4597-89ce-f6fc2b08fe51" />

Ref 28: 13979 packet is a POST packet.

<img width="733" height="680" alt="sqlmap v 147  It is a tool that proforms automated sql attacks" src="https://github.com/user-attachments/assets/4cc01360-8151-469b-9fe2-7ef1eeb7d43c" />

Ref 29: sqlmap v 147  It is a tool that proforms automated sql attacks.

<img width="1014" height="722" alt="another post request on 14060, looks to be the sql attack happening" src="https://github.com/user-attachments/assets/27a25c94-84bf-4e51-9868-9b95277a1130" />

Ref 29: Another post request on 14060, looks to be the sql attack happening.

<img width="1014" height="763" alt="decoding shows sgl attack, thier objective is to open up a shell to read a file etc passwd" src="https://github.com/user-attachments/assets/f1cbd219-8638-4325-9463-98ceec963f89" />

Ref 30: Decoding shows sgl attack, thier objective is to open up a shell to read a file etc/passwd.

<img width="965" height="14" alt="last post request from  4" src="https://github.com/user-attachments/assets/4aea3576-9b9a-4cc1-bfba-4672349c0273" />

Ref 31: last post request from .4.

<img width="1021" height="17" alt="Focusing on POST req from  4" src="https://github.com/user-attachments/assets/d4173edd-25a2-40c1-9b68-7ba0402e18c7" />

Ref 32: Focusing on POST req from .4.

<img width="968" height="10" alt="This POST has an upload, this is on packet 16102" src="https://github.com/user-attachments/assets/438b5dfa-f90a-4049-bf51-afc5637364bd" />

Ref 33: This POST has an upload, this is on packet 16102.

<img width="746" height="763" alt="attacker clicked on editprofile, then upload, then uploaded dbfunctions php" src="https://github.com/user-attachments/assets/dd2ae8ab-b08b-440e-b6df-61b40623512e" />

Ref 34: Attacker clicked on editprofile, then upload, then uploaded dbfunctions php.

<img width="716" height="412" alt="attacker clicked upload and the receiver confirmed" src="https://github.com/user-attachments/assets/d020c4ba-4a6f-4921-9228-17df6e176aad" />

Ref 35: Attacker clicked upload and the receiver confirmed.

<img width="966" height="12" alt="GET UPLOAD this attack worked and shows at packet 16134" src="https://github.com/user-attachments/assets/628d692c-b2c9-491f-bcf2-6508688cc4a7" />

Ref 36: GET UPLOAD this attack worked and shows at packet 16134.

<img width="426" height="187" alt="attacker uses both commands ID and WHOAMI" src="https://github.com/user-attachments/assets/2170dcf7-2ecc-4566-b32a-628ffc9396ba" />

Ref 37: Attacker uses both commands ID and WHOAMI.

<img width="968" height="15" alt="another GET on packet 16201" src="https://github.com/user-attachments/assets/52b3afa4-9165-4bcb-ab84-e2f65b9fef8a" />

Ref 38: Another GET on packet 16201.

<img width="743" height="719" alt="encoded will decode" src="https://github.com/user-attachments/assets/55b80b23-00fd-4eb5-92f9-87cdd7802226" />

Ref 39: This is encoded will use urldecoder.online.

<img width="1021" height="765" alt="using python  connection on 10 251 96 4 port 4422 they want to call bin, sh, i" src="https://github.com/user-attachments/assets/9460d9ad-22f3-42ce-8294-d24910fbf532" />

Ref 40: using python  connection on 10 251 96 4 port 4422 they want to call bin/sh/i.

<img width="968" height="44" alt="connection attempt with 3 way handshake with call back towards ip  4 on port 4422  " src="https://github.com/user-attachments/assets/d7ecf7dd-f832-4d1a-a97e-c6b718a0d371" />

Ref 41: Connection attempt with 3 way handshake with call back towards ip  4 on port 4422.

<img width="744" height="718" alt="attacker using directories using discovery commands" src="https://github.com/user-attachments/assets/f8d086a0-f004-4a70-a34b-3e2003cc886e" />

Ref 42: Attacker using directories using discovery commands.

Summary: 

IP: 10.251.96.5

Username: www-data

Hostname: bob-appserver


Port Scan Activity

Start: 2021-02-07 16:33:06 (UTC)

End: 2021-02-07 16:33:06 (UTC)

Source: 10.251.96.4

Destination: 10.251.96.5 (22/80 opened)


Applications used by 10.251.96.4

App 1: Gobuster 3.0.1

Start: 2021-02-07 16:34:05

End: 2021-02-07 16:34:06

App 2: sqlmap 1.4.7

Start: 2021-02-07 16:36:17

End: 2021-02-07 16:37:28


Successful Web Shell Upload

Name:dbfunctions.php

Start: 2021-02-07 16:40:39

Source: 10.251.96.4

Destination: 10.251.96.5


Commands ran by 10.251.96.4 via web shell id, whoami, python script for callback.


Successful callback to 10.251.96.4:4422 via TCP reverse shell from 10.251.96.5


Start: 2021-02-07 16:42:35


Commands ran from the webserver via reverse TCP shell

bash -i, whoami, cd, ls, python and rm db

Last observed activity from 10.251.96.4 was on 2021-02-07 16:45:56

End.
