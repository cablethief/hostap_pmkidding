# hostap_pmkidding
A patch to make Hostap return a PMKID so it can be cracked. 

# Usage

```sh
git clone git://w1.fi/hostap.git
cd hostap
# Grab the config from Hostapd-mana cause I am lazy and it has most of the stuff I want.
curl -o hostapd/.config 'https://raw.githubusercontent.com/Cablethief/hostapd-mana/master/hostapd/.config' 
curl -o give_pmkid.patch 'https://raw.githubusercontent.com/Cablethief/hostap_pmkidding/master/give_pmkid.patch'
git apply give_pmkid.patch
make -C hostapd
```

Or you can grab an already compiled hostapd from the releases:
https://github.com/Cablethief/hostap_pmkidding/releases
