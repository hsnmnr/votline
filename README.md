# votline

Votline AKA Vote Online consists of 4 Provencial servers Punjab, Sindh, KPK and Balochistan, with each server divided in 2 sub-servers called Part Servers (representing lower and upper parts of province) and one Federal server that connects to all provincial servers. For information sharing between servers and client-server Socket Programming is used with TCP protocol.

The structure of application is as follows:

1- Voter add vote info that is sent to Federal Server.

2- Federal Communicate the vote info to The Respected Provincial Server.

3- Provincial Server communicate the info to respected Part Server (lower or upper).

4- Once the Part Server gets the vote. It saves the Vote Data in at "./files/part.json" file, and send the successful message to Its Provincial Server.

5- Provincial Server receive the response save the data at "./files/part.json" file, and send the successful message to Federal Server.

6- In the end Federal Server saves the vote data at "./files/part.json" file, and send the successful message to Voter.
