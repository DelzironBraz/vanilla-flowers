# Vanilla Flowers

## Passo a Passo

Faz backup da pasta do apache atual
```shell
sudo cp -r /var/www/html /var/www/html_backup
```

Remove o que tem no diretório
```shell
sudo rm -rf /var/www/html/*
```

Faz o clone do repositório no diretório
```shell
cd /var/www/html
sudo git clone https://github.com/seu-usuario/seu-repositorio.git .
```

Após substituir o arquivo, reinicie o serviço do apache
```shell
sudo systemctl restart apache2
```
