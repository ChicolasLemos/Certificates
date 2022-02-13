# Certificates
```
apt install easy-rsa
cp -r /usr/share/easy-rsa/ /etc/
cd /etc/easy-rsa/
nano openssl-easyrsa.conf
mv vars.example vars
nano vars
   > “ca_only” to “org”
   > Put your information
./easyrsa init-pki
./easyrsa build-ca
./easyrsa build-server-full domain nopass
Copy the certificates to 
   > "/etc/ssl/certs/domain.crt"
   > "/etc/ssl/private/domain.key" 
```
