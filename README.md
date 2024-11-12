# Setting Up My DigitalOcean Droplet with SSH Access

This README outlines the steps I followed to provision a server on DigitalOcean, create an SSH key on my local machine, add the public key to the server, and securely connect via SSH. This guide should be helpful if you're looking to replicate this setup.

---

## Steps I Took to Provision a DigitalOcean Droplet

1. **Logged into DigitalOcean** and navigated to the Droplets section. I clicked on **Create Droplet** to start a new server.
2. **Selected Ubuntu** as my OS (I went with this because it’s widely supported and easy to configure).
3. **Chose the droplet’s specifications**: I picked a plan that matched my needs and a datacenter close to me to keep latency low.
4. **Chose SSH key authentication** for added security over a password. Since I hadn’t yet created an SSH key, I left this section for now and planned to add it later.
5. **Finished creating the droplet** by naming it and confirming my selections. Within a few seconds, my server was up and running, and I noted down the droplet’s IP address.

---

## Creating My SSH Key Pair

Since I needed an SSH key pair for secure access, I created one on my local machine:

1. Opened my terminal and ran the following command to create a new SSH key pair:

   ```bash
   ssh-keygen -t rsa -b 4096 -C "my_email@example.com"

   ```

2. ssh Into my server using
   ```bash
       ssh user@host
   ```

## Project Link

https://roadmap.sh/projects/ssh-remote-server-setup
