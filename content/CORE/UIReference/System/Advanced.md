---
title: "Advanced"
description: "Describes the System > Advanced screen on TrueNAS CORE."
weight: 40
tags:
- coreconfiguration
- coresettings
---

**System > Advanced** contains advanced options for configuring system settings.

{{< hint type=important >}}
These options have reasonable defaults in place.
Make sure you are comfortable with ZFS, FreeBSD, and system [configuration backup and restoration]({{< relref "/content/CORE/CORETutorials/SystemConfiguration/UsingConfigurationBackups.md" >}}) before making any changes.
{{< /hint >}}

![System Advanced13](/images/CORE/13.0/SystemAdvanced13.png "Advanced Settings")

{{< include file="content/_includes/SystemAdvancedFields.md" type="page" >}}

**SAVE DEBUG** generates text files that contain diagnostic information.

{{< taglist tag="coreconfiguration" limit="10" >}}
