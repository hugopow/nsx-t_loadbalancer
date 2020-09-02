# nsx-t_loadbalancer
Postman collection and environment that contains the necessary calls and variables to successfully configure the NSX-T load balancer services.

Variable: nsx_vip	Description: nsx-t manager cluster virtual ip

Variable: nsx-manager-user	Description: nsx-t manager username, usually admin

Variable: nsx-manager-password	Description: nsx-t manager password

Variable: vcd-public-ip	Description: public ip address for the vcd service to be configured on the load balancer

Variable: tenant-app-public-ip	Description: public ip address for the tenant app service to be configured on the load balancer

Variable: vcd-cert-name	Description: a name for the imported vcd http certificate

Variable: vcd-cert-private-key	Description: vcd http certificate private key in pem format, the APIs only accept single line and no spaces in the certificate chain, use \n as an end of line character.

for example: —–BEGIN RSA PRIVATE KEY—–\n<private key>\n—–END RSA PRIVATE KEY—–
  
Variable: vcd-cert-passphrase	Description: vcd private key passphrase

Variable: vcd-certificate	Description: vcd http certificate in pem format, the APIs only accept single line and no spaces in the certificate chain, use \n as an end of line character.

For example: —–BEGIN CERTIFICATE—–\nMIIGADCCBOigAwIBAgIRALUVXndtVGMeRM1YiMqzBCowDQYJKoZIhvcNAQELBQAw\ngY8xCzAJBgNVBAYTAkdCMRswGQYDVQQIExJHcmVhdGVyIE1hbmNoZXN0ZXIxEDAO\nBgNVBAcTB1NhbGZvcmQxGDAWBgNVBAoTD1NlY3RpZ28gTGltaXRlZDE3MDUGA1UE\nAxMuU2VjdGlnbyBSU0EgRG9tYWluIFZhbGlkYXRpb24gU2VjdXJlIFNlcnZlciBD\nQTAeFw0xOTA4MjMwMDAwMDBaFw0yMDA4MjIyMzU5NTlaMFUxITAfBgNVBAsTGERv\nbWFpbiBDb250cm9sIFZhbGlkYXRlZDEUMBIGA1UECxMLUG9zaXRpdmVTU0wxGjAY\nBgNVBAMTEXZjbG91ZC52bXdpcmUuY29tMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8A\nMIIBCgKCAQEAqh9sn6bNiDmmg3fJSG4zrK9IbrdisALFqnJQTkkErvoky2ax0RzV\n/ZJ/1fNHpvy1yT7RSZbKcWicoxatYPCgFHDzz2JwgvfwQCRMOfbPzohTSAhrPZph\n4FOPnrF8iwGggTxp+/2/ixg0DjQZL32rc9ax1qEvSURt571hUE7uLkRbPrdbocSZ\n4c2atVh8K1fp3uBqEbAs0UyjW5PK3wIN5ZRFArxc5kiGW0btN1RmoWwOmuJkAtu7\nzuaAJcgr/UVb1PP+GgAvKdmikssB1MWQALTRHm7H2GJp2MlbyGU3ZROSPkSSaNsq\n4otCJxtvQze/lB5QGWj5V2B7YbNJKwJdXQIDAQABo4ICjjCCAoowHwYDVR0jBBgw\nFoAUjYxexFStiuF36Zv5mwXhuAGNYeEwHQYDVR0OBBYEFNhZaRisExXrYrqfIIm6\n9TP8JrqwMA4GA1UdDwEB/wQEAwIFoDAMBgNVHRMBAf8EAjAAMB0GA1UdJQQWMBQG\nCCsGAQUFBwMBBggrBgEFBQcDAjBJBgNVHSAEQjBAMDQGCysGAQQBsjEBAgIHMCUw\nIwYIKwYBBQUHAgEWF2h0dHBzOi8vc2VjdGlnby5jb20vQ1BTMAgGBmeBDAECATCB\nhAYIKwYBBQUHAQEEeDB2ME8GCCsGAQUFBzAChkNodHRwOi8vY3J0LnNlY3RpZ28u\nY29tL1NlY3RpZ29SU0FEb21haW5WYWxpZGF0aW9uU2VjdXJlU2VydmVyQ0EuY3J0\nMCMGCCsGAQUFBzABhhdodHRwOi8vb2NzcC5zZWN0aWdvLmNvbTAzBgNVHREELDAq\nghF2Y2xvdWQudm13aXJlLmNvbYIVd3d3LnZjbG91ZC52bXdpcmUuY29tMIIBAgYK\nKwYBBAHWeQIEAgSB8wSB8ADuAHUAsh4FzIuizYogTodm+Su5iiUgZ2va+nDnsklT\nLe+LkF4AAAFsv3BsIwAABAMARjBEAiBat+l0e3BTu+EBcRJfR8hCA/CznWm1mbVl\nxZqDoKM6tAIgON6U0YoqA91xxpXH2DyA04o5KSdSvNT05wz2aa7zkzwAdQBep3P5\n31bA57U2SH3QSeAyepGaDIShEhKEGHWWgXFFWAAAAWy/cGw+AAAEAwBGMEQCIDHl\njofAcm5GqECwtjBfxYD7AFkJn4Ez0IGRFrux4ldiAiAaNnkMbf0P9arSDNno4hQT\nIJ2hUaIWNfuKBEIIkfqhCTANBgkqhkiG9w0BAQsFAAOCAQEAZCubBHRV+m9iiIeq\nCoaFV2YZLQUz/XM4wzQL+73eqGHINp6xh/+kYY6vw4j+ypr9P8m8+ouqichqo7GJ\nMhjtbXrB+TTRwqQgDHNHP7egBjkO+eDMxK4aa3x1r1AQoRBclPvEbXCohg2sPUG5\nZleog76NhPARR43gcxYC938OH/2TVAsa4JApF3vbCCILrbTuOy3Z9rf3aQLSt6Jp\nkh85w6AlSkXhQJWrydQ1o+NxnfQmTOuIH8XEQ2Ne1Xi4sbiMvWQ7dlH5/N8L8qWQ\nEPCWn+5HGxHIJFXMsgLEDypvuXGt28ZV/T91DwPLeGCEp8kUC3N+uamLYeYMKOGD\nMrToTA==\n—–END CERTIFICATE—–

Variable: ca-cert-name	Description: a name for the imported ca root certificate
Variable: ca-certificate	Description: ca root certificate in pem format, the APIs only accept single line and no spaces in the certificate chain, use \n as an end of line character.
Variable: vcd-node1-name	Description: the hostname for the first vcd appliance

Variable: vcd-node1-ip	Description: the dmz ip address for the first vcd appliance

Variable: vcd-node2-name	Description: the hostname for the second vcd appliance

Variable: vcd-node2-ip	Description: the dmz ip address for the second vcd appliance

Variable: vcd-node3-name	Description: the hostname for the third vcd appliance

Variable: vcd-node3-ip	Description: the dmz ip address for the third vcd appliance

Variable: tenant-app-node-name	Description: the hostname for the vrealize operations tenant app appliance

Variable: tenant-app-node-ip	Description: the dmz ip address for the vrealize operations tenant app appliance

Variable: tenant-app-cert-name	Description: a name for the imported tenant app certificate

Variable: tenant-app-cert-private-key	Description: tenant app certificate private key in pem format, the APIs only accept single line and no spaces in the certificate chain, use \n as an end of line character.

For example: —–BEGIN RSA PRIVATE KEY—–\n<private key>\n—–END RSA PRIVATE KEY—–

Variable: tenant-app-cert-passphrase	Description: tenant app private key passphrase

Variable: tenant-app-certificate	Description: tenant app certificate in pem format, the APIs only accept single line and no spaces in the certificate chain, use \n as an end of line character.

For example: —–BEGIN CERTIFICATE—–\nMIIGADCCBOigAwIBAgIRALUVXndtVGMeRM1YiMqzBCowDQYJKoZIhvcNAQELBQAw\ngY8xCzAJBgNVBAYTAkdCMRswGQYDVQQIExJHcmVhdGVyIE1hbmNoZXN0ZXIxEDAO\nBgNVBAcTB1NhbGZvcmQxGDAWBgNVBAoTD1NlY3RpZ28gTGltaXRlZDE3MDUGA1UE\nAxMuU2VjdGlnbyBSU0EgRG9tYWluIFZhbGlkYXRpb24gU2VjdXJlIFNlcnZlciBD\nQTAeFw0xOTA4MjMwMDAwMDBaFw0yMDA4MjIyMzU5NTlaMFUxITAfBgNVBAsTGERv\nbWFpbiBDb250cm9sIFZhbGlkYXRlZDEUMBIGA1UECxMLUG9zaXRpdmVTU0wxGjAY\nBgNVBAMTEXZjbG91ZC52bXdpcmUuY29tMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8A\nMIIBCgKCAQEAqh9sn6bNiDmmg3fJSG4zrK9IbrdisALFqnJQTkkErvoky2ax0RzV\n/ZJ/1fNHpvy1yT7RSZbKcWicoxatYPCgFHDzz2JwgvfwQCRMOfbPzohTSAhrPZph\n4FOPnrF8iwGggTxp+/2/ixg0DjQZL32rc9ax1qEvSURt571hUE7uLkRbPrdbocSZ\n4c2atVh8K1fp3uBqEbAs0UyjW5PK3wIN5ZRFArxc5kiGW0btN1RmoWwOmuJkAtu7\nzuaAJcgr/UVb1PP+GgAvKdmikssB1MWQALTRHm7H2GJp2MlbyGU3ZROSPkSSaNsq\n4otCJxtvQze/lB5QGWj5V2B7YbNJKwJdXQIDAQABo4ICjjCCAoowHwYDVR0jBBgw\nFoAUjYxexFStiuF36Zv5mwXhuAGNYeEwHQYDVR0OBBYEFNhZaRisExXrYrqfIIm6\n9TP8JrqwMA4GA1UdDwEB/wQEAwIFoDAMBgNVHRMBAf8EAjAAMB0GA1UdJQQWMBQG\nCCsGAQUFBwMBBggrBgEFBQcDAjBJBgNVHSAEQjBAMDQGCysGAQQBsjEBAgIHMCUw\nIwYIKwYBBQUHAgEWF2h0dHBzOi8vc2VjdGlnby5jb20vQ1BTMAgGBmeBDAECATCB\nhAYIKwYBBQUHAQEEeDB2ME8GCCsGAQUFBzAChkNodHRwOi8vY3J0LnNlY3RpZ28u\nY29tL1NlY3RpZ29SU0FEb21haW5WYWxpZGF0aW9uU2VjdXJlU2VydmVyQ0EuY3J0\nMCMGCCsGAQUFBzABhhdodHRwOi8vb2NzcC5zZWN0aWdvLmNvbTAzBgNVHREELDAq\nghF2Y2xvdWQudm13aXJlLmNvbYIVd3d3LnZjbG91ZC52bXdpcmUuY29tMIIBAgYK\nKwYBBAHWeQIEAgSB8wSB8ADuAHUAsh4FzIuizYogTodm+Su5iiUgZ2va+nDnsklT\nLe+LkF4AAAFsv3BsIwAABAMARjBEAiBat+l0e3BTu+EBcRJfR8hCA/CznWm1mbVl\nxZqDoKM6tAIgON6U0YoqA91xxpXH2DyA04o5KSdSvNT05wz2aa7zkzwAdQBep3P5\n31bA57U2SH3QSeAyepGaDIShEhKEGHWWgXFFWAAAAWy/cGw+AAAEAwBGMEQCIDHl\njofAcm5GqECwtjBfxYD7AFkJn4Ez0IGRFrux4ldiAiAaNnkMbf0P9arSDNno4hQT\nIJ2hUaIWNfuKBEIIkfqhCTANBgkqhkiG9w0BAQsFAAOCAQEAZCubBHRV+m9iiIeq\nCoaFV2YZLQUz/XM4wzQL+73eqGHINp6xh/+kYY6vw4j+ypr9P8m8+ouqichqo7GJ\nMhjtbXrB+TTRwqQgDHNHP7egBjkO+eDMxK4aa3x1r1AQoRBclPvEbXCohg2sPUG5\nZleog76NhPARR43gcxYC938OH/2TVAsa4JApF3vbCCILrbTuOy3Z9rf3aQLSt6Jp\nkh85w6AlSkXhQJWrydQ1o+NxnfQmTOuIH8XEQ2Ne1Xi4sbiMvWQ7dlH5/N8L8qWQ\nEPCWn+5HGxHIJFXMsgLEDypvuXGt28ZV/T91DwPLeGCEp8kUC3N+uamLYeYMKOGD\nMrToTA==\n—–END CERTIFICATE—–

Variable: tier1-full-path	Description: the full path to the nsx-t tier1 gateway that will run the load balancer,

for example /infra/tier-1s/stage1-m-ec01-t1-gw01

Variable: vcd-dmz-segment-name	Description: the portgroup name of the vcd dmz portgroup,

for example stage1-m-vCDFront

Variable: allowed_ip_a	Description: an ip address that is allowed to access the /provider URI and the admin API

Variable: allowed_ip_b	Description: an ip address that is allowed to access the /provider URI and the admin API
