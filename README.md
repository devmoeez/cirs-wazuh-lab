# CIRS: Cyber Incident Response System (Operation Weak Link)

A hands-on incident response lab. A Wazuh SIEM on Ubuntu monitors a target environment while Kali Linux plays the attacker. Attacks are launched, detected, triaged and documented following an incident response lifecycle.

Capstone project, BS Cybersecurity, UMT Lahore.

## **1. Lab Architecture**

| Machine | Role |
|---|---|
| Ubuntu Server | Wazuh manager, indexer and dashboard |
| Target host | Wazuh agent installed |
| Kali Linux | Attacker |

## **2. Scenarios Covered**

- Brute-force login attempts
- Network reconnaissance and port scanning
- File integrity changes on monitored paths
- Privilege escalation indicators

Each scenario includes the attack command, the Wazuh alert generated, the rule ID and the response action.

## **3. Incident Response Phases**

1. Preparation
2. Detection and analysis
3. Containment
4. Eradication and recovery
5. Lessons learned

## **4. Setup**

```bash
# On Ubuntu (Wazuh all-in-one)
curl -sO https://packages.wazuh.com/4.x/wazuh-install.sh
sudo bash ./wazuh-install.sh -a
```

Then install the Wazuh agent on the target host and register it with the manager.

## **5. Deliverables**

- Full technical report
- Presentation slides
- Alert screenshots and rule mappings

## **6. Author**

**Moeez Hashmi**
