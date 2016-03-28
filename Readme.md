Dieses Repository definiert die Anwendung der kbu_ansible_roles in der KBU-Infrastruktur.
Es dokumentiert damit die tatsächliche Serverkonfiguration.

#### Inhalt

Das Repository besteht dabei aus den Dateien und Ordnern:

* [roles](roles) bindet den Basis-Rollensatz ein
* [hosts](hosts) ist das Ansible Inventory - hier sind alle Server definiert
* [playbook.yml](playbook.yml) ist das Ansible Playbook. Es definiert, welche Rollen wie auf welchen Server angewendet werden.

#### Ausführen
`ansible-playbook -i hosts -u <Dein Server Benutzer> --check playbook.yml`

`--check` sorgt dafür, dass die Konfiguration lediglich überprüft wird. Zur Anwendung musst Du diesen Parameter entfernen.

