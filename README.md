⚠️ Hacking em Redes Sociais – Fins Educacionais

Atenção: Este repositório é destinado exclusivamente para fins educacionais, CTFs e testes em ambientes controlados.
O objetivo é compreender vulnerabilidades comuns em redes sociais e como preveni-las.
O uso indevido destas informações é crime.

🔐 Brute Force e Phishing em Redes Sociais – Estudo de Ferramentas

SET (Social-Engineer Toolkit):
Framework poderoso para engenharia social, com suporte à criação de páginas falsas de login para fins de teste.

![descrição](/setoolkit.png)

https://github.com/trustedsec/social-engineer-toolkit

🌐 Redirecionando com Ngrok e SEToolkit
Se você tá rodando o SEToolkit localmente e quer expor a página falsa pra fora da rede (tipo pra testes em ambiente controlado), o Ngrok é a ferramenta chave. Ele cria um túnel HTTP pro seu localhost.

1. Em outro terminal, rode o Ngrok:
    ```ngrok http 80 ```

2. O Ngrok vai gerar um link tipo:
    ``` https://12ab-xx-xx-xx-xx.ngrok.io ```
É esse link que você compartilha para testar a página em outro dispositivo.
https://ngrok.com/downloads/linux
   
Zphisher:
Ferramenta para automação de ataques de phishing em múltiplas plataformas sociais, com modelos prontos e fácil integração.

![descrição](/workflow.gif)

https://github.com/htr-tech/zphisher

Hydra:
Ferramenta de força bruta para testar senhas fracas em logins públicos ou APIs mal protegidas.
Permite realizar autenticações em massa com combinações de usuário e senha.

Exemplo básico de uso com Hydra (web login):

    hydra -l usuário -P senhas.txt facebook.com http-post-form "/login:email=^USER^&pass=^PASS^:F=login_error"  

https://github.com/vanhauser-thc/thc-hydra

🕵️‍♂️ Keyloggers e Sniffers para Captura de Credenciais

🔑 Keyloggers:

Logkeys:
Keylogger de linha de comando para Linux, simples e direto. Ideal para demonstrações locais.

LKL (Linux KeyLogger):
Keylogger leve que roda em modo usuário e grava pressionamentos de tecla.

PyKeylogger:
Escrito em Python, com suporte ao envio remoto de logs por e-mail. Útil em laboratórios educacionais para mostrar exfiltração de dados.

🌐 Sniffers de Tráfego:

Wireshark:
O mais conhecido analisador de pacotes. Permite interceptar e analisar tráfego em texto claro (HTTP, FTP, etc.).

Ettercap:
Excelente para ataques MITM (Man-in-the-Middle). Pode interceptar e modificar tráfego em redes locais.

dsniff:
Conjunto de ferramentas de sniffing para capturar tráfego de protocolos como FTP, Telnet e HTTP.
