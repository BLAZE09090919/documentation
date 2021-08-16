---
title: "Settings"
weight: 50
---

{{< toc >}}

The **Administration** page shows additional system details and offers a variety of TrueCommand configuration options.
This page is available to users with administrator permissions by opening the **Configure** <i class="material-icons" aria-hidden="true" title="Settings">settings</i> menu and clicking *Administration*.
The page is organized into **About**, **Certificates**, and **Configuration** tabs.

{{< tabs "Administration Tabs" >}}
{{< tab "About" >}}
The **About** tab contains the current TrueCommand system ID and version, license details, and contact information for iXsystems.

![AdministrationAbout](/images/TrueCommand/1.3/AdministrationAbout.png "Administration Configuration")

### Updating the License

You can expand TrueCommand to monitor more disks by upgrading or purchasing a license from iXsystems.
Clicking *GET A LICENSE* opens a new browser tab to purchase a TrueCommand license.
You can also contact iXsystems to upgrade the current license.

After you purchase or upgrade the license, you must upload the new license to TrueCommand.
Click *Browse…* to open a file browser on your local system.
Select the new license file to upload and click *UPLOAD LICENSE* to apply the new license to TrueCommand.
{{< /tab >}}
{{< tab "Certificates" >}}
The **Certificates** tab shows the certificates and Certificate Authorities (CAs) TrueCommand uses and has options to upload or import a certificate or CA.

![AdministrationCertificates](/images/TrueCommand/1.3/AdministrationCertificates.png "Administration: Certificates")

Clicking *Browse...* opens a dialog to upload a file from the local system.
Selecting *Plain text* allows you to copy and paste the file raw text instead of uploading a file.
{{< /tab >}}
{{< tab "Configuration" >}}
The Configuration tab contains options to configure various features of TrueCommand.

![Administration About](/images/TrueCommand/1.3/AdministrationConfiguration.png "Administration: Configuration")

Changing any options requires clicking *SAVE* to save the new system configuration.
To reset fields back to their previous values, click *CANCEL*.

General options include how frequently TrueCommand measures systems statistics, how long to store system statistics, and the number of database backups from an iXsystems NAS to store.

### SSL options

{{< hint info >}}
This feature is only available for local installations or containerized TrueCommand deployments.
{{< /hint >}}

{{< include file="static/includes/TrueCommand/2.0/TrueCommandSSL.md.part" markdown="true" >}}

### Alert Options

You can adjust the alert levels that TrueCommand shows from a connected NAS to tune the system messages shown according to your use case.
Choose an alert category to ignore.
Multiple categories can be selected.

### LDAP

{{< include file="static/includes/TrueCommand/2.0/TrueCommandLDAP.md.part" markdown="true" >}}


Enabling *Allow LDAP user creation* means TrueCommand creates user accounts when someone logs in to the User Interface with their LDAP credentials.
*JOIN TEAM* automatically adds LDAP users to specific TrueCommand teams.

### Telemetry

TrueCommand reports some basic usage telemetry back to iXsystems for product improvement analysis. These metrics are completely anonymous.

Click the *PREVIEW* button to see exactly what your system is sending.<br>
Check the *Disable Telemetry* check box and click the *SAVE* button to disable this feature.

{{< /tab >}}
{{< /tabs >}}
