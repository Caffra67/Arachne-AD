## Connect to AD -> Samba Winbind
i used winbind because SSSD and Realmd don't work for me


```
sudo apt update -y && sudo apt full-upgrade -y && sudo apt autoremove -y && sudo apt autoclean -y
```

```
sudo apt -y install winbind libpam-winbind libnss-winbind krb5-config samba-dsdb-modules samba-vfs-modules
```

add home directory on login 
```
sudo pam-auth-update
```

nsswitch.conf ipasswd: and group: winbind to work 

---

```
sudo mv /etc/samba/smb.conf /etc/samba/smb.conf.org
```

smb.conf add:
```
[global]
	kerberos method = secrets and keytab
	realm = AD.ARACHNE.COM
	workgroup = ARACHNE

	security = ads
	template shell = /bin/bash
	winbind enum groups = Yes
	winbind enum users = Yes	
	winbind separator = +

	idmap config * : rangesize = 1000000
	idmap config * : range = 1000000-19999999
	idmap config * : backend = autorid
```

resolv.conf add:
```
nameserver 10.0.0.X
```

Connect to AD
```
sudo net ads join -U Administrator
```
Source:
1. Michael Waterman, Domain Join Ubuntu 22.04 to Active Directory, https://michaelwaterman.nl/2022/10/02/domain-join-ubuntu-22-04-to-active-directory/
