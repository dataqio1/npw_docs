# Linux Install

## 54VVG-872U7-75CC4-3CC18-60882-D6837Download software

```
# url will be sent in the email along with license key.

wget url

eg : wget https://dataops-store.s3.amazonaws.com/dataops_server.zip
```

```
#unzip the zip file
unzip dataops_server.zip
```

```
cd dataops_server
```

### Set License Name and License Key

**Edit .env** file and update following two properties (from the values you received in the email ). Replace the default value of the LICENSE\_NAME with the value received in email.

```
LICENSE_NAME=<Name>
LICENSE_KEY=<key>
```

### Set Server URL

```
HOST_URL=< URL ex: dv.example.com or if there is no URL can also set IP addr>
```

{% hint style="info" %}
If https keys are provided, set the HOST\_URL to **https**://\<server URL>
{% endhint %}

### Start the server

Start the server either with sudo or user with admin privileges.

```
 ./start_server.sh
```

### Open the browser and go to the url : http://\<HOST\_URL>

Note : Host is the server url or the ip address.

{% hint style="warning" %}
Do not use localhost in the url.
{% endhint %}

### **Login and enable LDAP settings**

Login with default users sent in the email along with the License key.

Note : For LDAP integration Go to Settings --> Properties and fill up the LDAP server details. Restart the server using ./restart\_server.sh for the changes to take effect.

![](<../../.gitbook/assets/image (42).png>)

![](<../../.gitbook/assets/image (43).png>)
