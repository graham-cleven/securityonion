### 2.3.210-20230202 ISO image built on 2023/02/02



### Download and Verify

2.3.210-20230202 ISO image:  
https://download.securityonion.net/file/securityonion/securityonion-2.3.210-20230202.iso

MD5: ED38C36DBE40509FC5E87D82B07141C0  
SHA1: EDEBDBE75FF34DAD87E141CA8F8614295ED23FB5  
SHA256: 30068D4B910E83B63287EAB98E49497A584BAE07854367716813E5D610D3E5E3 

Signature for ISO image:  
https://github.com/Security-Onion-Solutions/securityonion/raw/master/sigs/securityonion-2.3.210-20230202.iso.sig

Signing key:  
https://raw.githubusercontent.com/Security-Onion-Solutions/securityonion/master/KEYS  

For example, here are the steps you can use on most Linux distributions to download and verify our Security Onion ISO image.

Download and import the signing key:  
```
wget https://raw.githubusercontent.com/Security-Onion-Solutions/securityonion/master/KEYS -O - | gpg --import -  
```

Download the signature file for the ISO:  
```
wget https://github.com/Security-Onion-Solutions/securityonion/raw/master/sigs/securityonion-2.3.210-20230202.iso.sig
```

Download the ISO image:  
```
wget https://download.securityonion.net/file/securityonion/securityonion-2.3.210-20230202.iso
```

Verify the downloaded ISO image using the signature file:  
```
gpg --verify securityonion-2.3.210-20230202.iso.sig securityonion-2.3.210-20230202.iso
```

The output should show "Good signature" and the Primary key fingerprint should match what's shown below:
```
gpg: Signature made Thu 02 Feb 2023 08:31:18 PM EST using RSA key ID FE507013
gpg: Good signature from "Security Onion Solutions, LLC <info@securityonionsolutions.com>"
gpg: WARNING: This key is not certified with a trusted signature!
gpg:          There is no indication that the signature belongs to the owner.
Primary key fingerprint: C804 A93D 36BE 0C73 3EA1  9644 7C10 60B7 FE50 7013
```

Once you've verified the ISO image, you're ready to proceed to our Installation guide:  
https://docs.securityonion.net/en/2.3/installation.html
