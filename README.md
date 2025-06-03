⚠️ Hacking em Redes Sociais – Fins Educacionais

Atenção: Este repositório é destinado exclusivamente para fins educacionais, CTFs e testes em ambientes controlados.
O objetivo é compreender vulnerabilidades comuns em redes sociais e como preveni-las.
O uso indevido destas informações é crime.

🔐 Brute Force e Phishing em Redes Sociais – Estudo de Ferramentas

SET (Social-Engineer Toolkit):
Framework poderoso para engenharia social, com suporte à criação de páginas falsas de login para fins de teste.

Zphisher:
Ferramenta para automação de ataques de phishing em múltiplas plataformas sociais, com modelos prontos e fácil integração.
![descrição](/workflow.gif)

Hydra:
Ferramenta de força bruta para testar senhas fracas em logins públicos ou APIs mal protegidas.
Permite realizar autenticações em massa com combinações de usuário e senha.

Exemplo básico de uso com Hydra (web login):

    hydra -l usuário -P senhas.txt facebook.com http-post-form "/login:email=^USER^&pass=^PASS^:F=login_error"

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
