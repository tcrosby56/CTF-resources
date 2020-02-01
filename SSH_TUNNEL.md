# SSH Tunnel to see local resources through a SSH connection

(This allows you to view resources such as a webserver hosted on a VM locally or in another VM)

    $ ssh -L <local_port>:<local_IP>:<remote_port> <username>@<remote_host>
      <local_port> = the port you want to use to view resources
      <local_IP> = the IP to forward to (typically 127.0.0.1)
      <remote_port> = the port to forward from (e.g. - webserver on port 80)
      <username> = the username you use to login to the vm
      <remote_host> = the remote host IP or FQDN

      Example:
    $ ssh -L 8080:127.0.0.1:80 test@test.testing.com
            OR
    $ ssh -L 8080:127.0.0.1:80 test@192.168.1.34

## Additional Resources:
  [Cyber Plumber's Handbook](https://cph.opsdisk.com/)
