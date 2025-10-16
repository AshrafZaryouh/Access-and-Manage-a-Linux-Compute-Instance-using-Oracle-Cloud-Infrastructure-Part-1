# Approach 1: Connect via SSH to the Compute Instance Public IP Address using a SSH Private Key with the macOS Terminal

In this approach, we will connect to a Linux instance using SSH and the public IP address that is provided by OCI to connect directly to the instance using the macOS terminal.

<img width="2338" height="1710" alt="Access-Manage-Linux-Instance-200" src="https://github.com/user-attachments/assets/b60a2843-ea8b-47ae-92d8-c0980a73ab7d" />

+ Run the following commands.

1 - Use the command line interface (CLI) to navigate to the folder where the public and private keys are stored.

```
cd Downloads
cd MyFreeInstanceKeys
ls -l
```

2 - Connect to the instance using the SSH command where you specify the private key.
3 - Restrict permissions of the private key and make sure the access is restricted, before it can be used.

```
chmod 600 ssh-key-2024-01-31.key
```

4 - Connect to the instance using the SSH command where you specify the private key.

```
ssh -i ssh-key-2024-01-31.key opc@xxx.xxx.xxx.229
```

5 - Run the following command to verify the IP address.

```
ip a
```

6 - Verify the IP address.

<img width="1047" height="583" alt="Access-Manage-Linux-Instance-201" src="https://github.com/user-attachments/assets/e369e8a0-9096-421a-bfe3-51366f927b31" />

---

---
