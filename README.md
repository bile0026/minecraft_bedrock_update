# minecraft_bedrock_update

updates minecraft bedrock installation.

# How to use

Update variables if they vary in minecraft_bedrock_updates/defaults/main.yml. Specifically the version variable.
Make sure you set this to the version you want to upgrade to.

Also create a "hosts" file with your server name in the file.

Run with:
```ansible-playbook -i hosts update_minecraft.yml -u <username> -k -K```

It will prompt you for the user password and sudo password. Enter these when prompted.
You can also use "--key-file <keypath>" instead of "-k" for pubkey authentication.

# Possible Future Enhancements
* automatically get the most recent version without having to specify version