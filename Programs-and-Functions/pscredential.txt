PSCredential () {
    echo -e "\n\t[+] \$user = 'user'"
    echo -e "\t[+] \$pw = 'password'"
    echo -e "\t[+] \$secpw = ConvertTo-SecureString \$pw -AsPlainText -Force"
    echo -e "\t[+] \$cred = New-Object System.Management.Automation.PSCredential \$user, \$secpw"
    echo -e "\t[+] Invoke-Command -ComputerName localhost -Credential \$cred -ScriptBlock { whoami }"
}