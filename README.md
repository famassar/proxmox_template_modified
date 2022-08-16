# proxmox_template_modified
This is a simple update of the official Zabbix ProxMox VE template with the exclusion of unused vms<br>
<br>Sometimes you have some vms on your proxmox normally stopped (i.e. for test or occasional use).<br>
<br>With original template of Zabbix these vm are discovered but generate a lot of errors (for Zabbix the stopped vm are not ok)<br>
<br>In this template you insert the VM IDs for the stopped VM in the macros {$LXC.ID.EXCLUDE} and {$QEMU.ID.EXCLUDE} (i.e. 101 or (101|102) if you have more than one vm) and no other.
