## Progression for Lab3a-2

### Updating Ubuntu Before Installing Certbot.

I started by going back to the home directory and running `sudo apt update`. I did this before installing Certbot so the server had the latest package information.

![Updating Ubuntu before Certbot](./Screenshots/Screenshot%202026-07-11%20170356.png)

### Installing Certbot and the Apache Plugin.

I installed Certbot and the Apache plugin using `sudo apt install certbot python3-certbot-apache -y`. Certbot was needed so I could request an SSL certificate for my DuckDNS domain.

![Installing Certbot and Apache plugin](./Screenshots/Screenshot%202026-07-11%20170431.png)

### Checking the Certbot Version.

After installing Certbot, I checked the version to make sure it was installed properly. The terminal showed Certbot version `2.9.0`.

![Checking Certbot version](./Screenshots/Screenshot%202026-07-11%20170504.png)

### Starting the HTTPS Certificate Setup.

I ran Certbot with Apache for my DuckDNS domain, `davenict171.duckdns.org`. During this step, Certbot asked for an email address and agreement to the Let's Encrypt terms.

![Starting Certbot certificate setup](./Screenshots/Screenshot%202026-07-11%20170656.png)

### Certificate Successfully Created.

Certbot successfully received and deployed the SSL certificate for my DuckDNS domain. It also showed that HTTPS had been enabled for `https://davenict171.duckdns.org`.

![Certificate successfully created](./Screenshots/Screenshot%202026-07-11%20170720.png)

### Testing the Website with HTTPS.

I opened my DuckDNS domain in the browser using HTTPS. The website loaded successfully and the browser showed the lock icon, which meant the SSL certificate was working.

![Testing website with HTTPS](./Screenshots/Screenshot%202026-07-11%20170800.png)

### Testing Certificate Renewal.

I tested the renewal process using `sudo certbot renew --dry-run`. The result showed that the simulated renewal succeeded, so the certificate renewal setup was working properly.

![Testing certificate renewal](./Screenshots/Screenshot%202026-07-11%20170852.png)

### My Conclusion

In this lab, I added HTTPS to my Azure web server using Certbot and Let's Encrypt. I started by updating Ubuntu, then installed Certbot with the Apache plugin. After that, I used Certbot to request and install an SSL certificate for my DuckDNS domain.

Once the certificate was created, I tested the website in the browser using `https://davenict171.duckdns.org`. The page loaded correctly and the lock icon appeared, which showed that HTTPS was working. I also tested the renewal process with a dry run, and it succeeded.

This lab helped me understand how HTTPS is added to a website. It also showed me why SSL certificates are important, because they make the website connection more secure and trusted by the browser.
