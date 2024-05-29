### Step 1

Download the latest release of Cloudflare Tunnel under the releases tab as shown on the bottom right hand corner of this picture.

![releases Tab](https://github.com/BrutusBondBTC/cloudflared-startos/blob/main/releases.png?raw=true)

### Step 2

Under the System Tab of the Start9 operating system, click on "Sideload a Service."

![sideload service](https://github.com/BrutusBondBTC/cloudflared-startos/blob/main/sideload.png?raw=true)

### Step 3

In Cloudflare: Navigagte to Networks > Tunnels. Then click create a tunnel. Click next.

![create tunnel](https://github.com/BrutusBondBTC/cloudflared-startos/blob/main/tunnel.png?raw=true)


### Step 4

Click on your tunnel name.(eg. start9)

![click name](https://github.com/BrutusBondBTC/cloudflared-startos/blob/main/clickTunnel.png?raw=true)


### Step 5

Click "Edit"

![edit](https://github.com/BrutusBondBTC/cloudflared-startos/blob/main/edit.png?raw=true


### Step 6

copy the string of letters and numbers after word "install".  In this example, we would copy"eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTY5NDc4NTEsIm5iZiI6MTcxNjk0NzU1MSwicGF0aCI6Ii81Njc1NjgxLzI4NTg0NDg4Mi04YmJhMjAzYi0wNGVhLTRhNDItYjZhZC1kNGVhZmQxODdhYTQucG5nP1gtQW16LUFsZ29yaXRobT1BV1M0LUhNQUMtU0hBMjU2JlgtQW16LUNyZWRlbnRpYWw9QUtJQVZDT0RZTFNBNTNQUUs0WkElMkYyMDI0MDUyOSUyRnVzLWVhc3QtMSUyRnMzJTJGYXdzNF9yZXF1ZXN0JlgtQW16LURhdGU9MjAyNDA1MjlUMDE1MjMxWiZYLUFtei1FeHBpcmVzPTMwMCZYLUFtei1TaWduYXR1cmU9YjljMDY4NzBjZWZhOTIwMTMzNDlhZTY4NTk1ZGIzNTIzMzZlMjA0YjI0MzhmM2NjYTZlOTFmNjYwMGUwNDNkYyZYLUFtei1TaWduZWRIZWFkZXJzPWhvc3QmYWN0b3JfaWQ9MCZrZXlfaWQ9MCZyZXBvX2lkPTAifQ.fMihDAKKp2FLS-qit4DN7s5818FWt3dc0u" but your characters will be different.
  

![RadioKot's Photo](https://private-user-images.githubusercontent.com/5675681/285844882-8bba203b-04ea-4a42-b6ad-d4eafd187aa4.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTY5NDc4NTEsIm5iZiI6MTcxNjk0NzU1MSwicGF0aCI6Ii81Njc1NjgxLzI4NTg0NDg4Mi04YmJhMjAzYi0wNGVhLTRhNDItYjZhZC1kNGVhZmQxODdhYTQucG5nP1gtQW16LUFsZ29yaXRobT1BV1M0LUhNQUMtU0hBMjU2JlgtQW16LUNyZWRlbnRpYWw9QUtJQVZDT0RZTFNBNTNQUUs0WkElMkYyMDI0MDUyOSUyRnVzLWVhc3QtMSUyRnMzJTJGYXdzNF9yZXF1ZXN0JlgtQW16LURhdGU9MjAyNDA1MjlUMDE1MjMxWiZYLUFtei1FeHBpcmVzPTMwMCZYLUFtei1TaWduYXR1cmU9YjljMDY4NzBjZWZhOTIwMTMzNDlhZTY4NTk1ZGIzNTIzMzZlMjA0YjI0MzhmM2NjYTZlOTFmNjYwMGUwNDNkYyZYLUFtei1TaWduZWRIZWFkZXJzPWhvc3QmYWN0b3JfaWQ9MCZrZXlfaWQ9MCZyZXBvX2lkPTAifQ.fMihDAKKp2FLS-qit4DN7s5818FWt3dc0u_L_7ITtVg)

⚠ Handle this command carefully. It includes a sensitive token that allows the connector to run. Anyone with access to this token will be able to run the tunnel.


### Step 7

Paste this token into the token field of the Config "Customize Cloudflare Tunnel" tab. Then click SAVE and Start the service

### Step 8

Navigate back to the tunnels page on Cloudflare. Click the public hostname button.

[public hostname](https://github.com/BrutusBondBTC/cloudflared-startos/blob/main/publichostname.png?raw=true)


### Step 9

Click "add a public host name."

[add public host name](https://github.com/BrutusBondBTC/cloudflared-startos/blob/main/service.png?raw=true)

### Step 10

On the Public Hostname Page add a domain. You can also add a subdomain in the subdomain section(eg. ghost for the ghost app)

Under type, enter HTTP 

**The URL will depend on the service you are adding. 

![public hostmname](https://github.com/BrutusBondBTC/cloudflared-startos/blob/main/publiicHostPage.png?raw=true)

Say you want to add Ghost. Search for Ghost repository under https://github.com/orgs/Start9Labs/repositories

It can be found here: https://github.com/Start9Labs/ghost-startos

Next, click on the manifest.yaml file use the id for the program, in this example it is "ghost". It would be "btcpayserver" if we were exposing the btcpayserver app, but the ID is ghost in this example so we will intere "ghost.embassy:2368 in the URL field of the Public Hostname Page back on Cloudflare.

![ghost](https://github.com/BrutusBondBTC/cloudflared-startos/blob/main/ghost1.png?raw=true)

The number "2368" is the port number and I found it under the port-mapping. In this case on line 53 

![port](https://github.com/BrutusBondBTC/cloudflared-startos/blob/main/port.png?raw=true)

So our Public Hostname Page should look something like this:

![final homepage](https://github.com/BrutusBondBTC/cloudflared-startos/blob/main/template.png?raw=true)

Your domain will be different of course but it will look like this

*Type* HTTP

*URL* id.embassy:port_number

Then click save hostname.

After a few minutes you can access your website on the clearnet.





