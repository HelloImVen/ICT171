## Progression for Lab3a-1

### Opening the DuckDNS Website.

I started by opening the DuckDNS website. This service was used so I could create a domain name that points to my Azure web server instead of only using the public IP address.

![Opening DuckDNS website](./Screenshots/Screenshot%202026-07-11%20164822.png)

### Creating the DuckDNS Domain.

I created the DuckDNS domain `davenict171.duckdns.org` and set it to point to my Azure VM public IP address, `104.214.189.237`. This means the domain name should open the same website as the public IP address.

![Creating DuckDNS domain](./Screenshots/Screenshot%202026-07-11%20165058.png)

### Testing the Website Using the DuckDNS Domain.

I opened `davenict171.duckdns.org` in the browser and my ICT171 cloud web server page loaded successfully. This showed that the DuckDNS domain was pointing to my Azure VM correctly.

![Testing website using DuckDNS domain](./Screenshots/Screenshot%202026-07-11%20165607.png)

### Testing DNS Lookup.

I also tested DNS lookup from the terminal. In this screenshot, I accidentally used the example domain `yourdomain.duckdns.org`, so this was not the main proof for my own domain. I used the browser test and the `curl` test with `davenict171.duckdns.org` to confirm my real domain was working.

![Testing DNS lookup](./Screenshots/Screenshot%202026-07-11%20165649.png)

### Testing the DuckDNS Domain with `curl`.

I used `curl -I` with `http://davenict171.duckdns.org` to check the website response from the terminal. The result showed `HTTP/1.1 200 OK`, which confirmed that the domain was working and the Apache web server was responding correctly.

![Testing DuckDNS domain with curl](./Screenshots/Screenshot%202026-07-11%20170202.png)

### My Conclusion

In this lab, I used DuckDNS to create a domain name for my Azure cloud web server. Instead of only using the public IP address, I connected the domain `davenict171.duckdns.org` to my Azure VM public IP address.

After setting up the domain, I tested it in the browser and my ICT171 cloud web server page loaded successfully. I also used `curl -I` to check the server response, and it returned `HTTP/1.1 200 OK`. This showed that the domain name was correctly linked to my Azure VM and that the Apache web server was working through the DuckDNS address.

This lab helped me understand how a domain name can be connected to a cloud server. It also showed me why DNS is useful, because it lets people visit a website using a readable name instead of remembering the server IP address.
