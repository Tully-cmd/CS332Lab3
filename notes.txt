!curl download nessus
```
curl --request GET \
  --url 'https://www.tenable.com/downloads/api/v2/pages/nessus/files/Nessus-10.3.0-debian9_amd64.deb' \
  --output 'Nessus-10.3.0-debian9_amd64.deb'
```
!installing nessus

```
sudo dpkg -i Nessus-10.3.0-debian9_amd64.deb         
```
!running nessus

```
sudo systemctl start nessusd
```
!kali ip
```172.16.0.17```
!metasploitable ip
```172.16.0.22
