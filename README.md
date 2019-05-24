# DNS configuration Anonymity Linux Distribution Gateways #

Pointing /etc/resolv.conf to 127.0.0.1.

Whether a Anonymity Linux Distribution Gateway supports system DNS for its own
traffic in the clear or anonymized mainly depends on the Gateway's firewall.

Routing the workstation's system DNS through the anonymizer (also known as
Transparent DNS Proxy) or not is up to the Gateway's firewall as well.
## How to install `anon-gw-dns-conf` using apt-get ##

1\. Add [Whonix's Signing Key](https://www.whonix.org/wiki/Whonix_Signing_Key).

```
sudo apt-key --keyring /etc/apt/trusted.gpg.d/whonix.gpg adv --keyserver hkp://ipv4.pool.sks-keyservers.net:80 --recv-keys 916B8D99C38EAF5E8ADC7A2A8D66066A2EEACCDA
```

3\. Add Whonix's APT repository.

```
echo "deb http://deb.whonix.org buster main contrib non-free" | sudo tee /etc/apt/sources.list.d/whonix.list
```

4\. Update your package lists.

```
sudo apt-get update
```

5\. Install `anon-gw-dns-conf`.

```
sudo apt-get install anon-gw-dns-conf
```

## How to Build deb Package ##

Replace `apparmor-profile-torbrowser` with the actual name of this package with `anon-gw-dns-conf` and see [instructions](https://www.whonix.org/wiki/Dev/Build_Documentation/apparmor-profile-torbrowser).

## Contact ##

* [Free Forum Support](https://forums.whonix.org)
* [Professional Support](https://www.whonix.org/wiki/Professional_Support)

## Donate ##

`anon-gw-dns-conf` requires [donations](https://www.whonix.org/wiki/Donate) to stay alive!
