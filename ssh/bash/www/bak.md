```
id=$(tr -dc 'a-z0-9' </dev/urandom | head -c 5) && zip -rq "/tmp/${id}.zip" /var/www/html && ip=$(hostname -I | awk '{print $1}') && clear && echo "<id.zip> ${id}.zip" && echo && echo "Windows (PowerShell): scp ${USER}@${ip}:/tmp/${id}.zip ." && echo "Linux: scp ${USER}@${ip}:/tmp/${id}.zip ." && echo "macOS: scp ${USER}@${ip}:/tmp/${id}.zip ."
```
