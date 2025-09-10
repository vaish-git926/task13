# Task 13 – Free Cloud VM Setup and Interaction

This task demonstrates how to create, configure, and interact with a free cloud-based virtual machine (VM).  
I used **Google Cloud Platform (GCP) Compute Engine** for this exercise.

---

## Steps Performed
1. Created a VM instance in GCP Compute Engine (Ubuntu, e2-micro free tier).
2. Allowed SSH (TCP 22) and ICMP (ping) traffic via firewall.
3. Obtained VM Public IP: **34.63.127.14**
4. From Kali Linux:
   - Pinged the VM public IP → ✅ successful
   - Connected via SSH and ran `ip a`
   - Checked Kali’s public IP: **106.76.179.168**
5. From the VM:
   - Pinged Kali’s public IP
6. Shut down and terminated the VM instance.

---

## Repository Contents
- `task13_steps.txt` → Detailed step-by-step explanation of the process.
- `ping_from_kali_to_vm.png` → Screenshot of pinging VM public IP from Kali.
- `ssh_ip_a_on_vm.png` → Screenshot of SSH session with `ip a` command.
- `ping_from_vm_to_kali.png` → Screenshot of pinging Kali’s public IP from VM.

---

## Notes
- Firewall rules must allow both **SSH** and **ICMP** traffic for successful interaction.
- Depending on ISP/firewall settings, pinging the Kali machine from VM may or may not succeed.
- VM was properly shut down and deleted after completion.
