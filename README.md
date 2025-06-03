HACKING EM REDES SOCIAIS

⚠️ Este repositório tem fins educacionais, CTFs e testes em ambientes controlados e aborda testes de segurança em redes sociais, com foco em phishing e ataques de força bruta. 
O objetivo é entender vulnerabilidades comuns e como preveni-las. O uso indevido é crime.

🔐 Brute Force e Phishing em Redes Sociais – Estudo de Ferramentas

Ferramentas abordadas:
• SET (Social-Engineer Toolkit): framework poderoso para engenharia social, com suporte a criação de páginas falsas de login para fins de teste.
• Zphisher: automação de ataques de phishing em múltiplas plataformas sociais, com modelos prontos e fácil integração.
• Ferramenta de Brute Force (Hydra): usada para testar senhas fracas por força bruta em logins públicos ou APIs mal protegidas Ela permite realizar ataques de força bruta contra diversos serviços de login. Com os parâmetros certos, dá pra tentar autenticações em massa, simulando logins com combinações de usuário e senha.

Exemplo básico de uso (para web login):
hydra -l usuário -P senhas.txt facebook.com http-post-form "/login:email=^USER^&pass=^PASS^:F=login_error"

🕵️‍♂️ Keyloggers e Sniffers para Captura de Credenciais

Além de ataques de força bruta e phishing, também é possível estudar a captura de credenciais através de keyloggers e sniffers de rede:

🔑 Keyloggers:
• Logkeys: keylogger de linha de comando para Linux, simples e direto. Pode registrar tudo o que é digitado no teclado, ideal para demonstrações locais.
• LKL (Linux KeyLogger): outra opção leve e discreta, que roda em modo usuário e grava pressionamentos de tecla.
• PyKeylogger: escrito em Python, com suporte a envio remoto de logs por e-mail. Pode ser útil em laboratórios educacionais para mostrar exfiltração de dados.

🌐 Sniffers de tráfego:
• Wireshark: o mais conhecido analisador de pacotes. Permite interceptar e analisar tráfego em texto claro (HTTP, FTP, etc.), inclusive logins não criptografados.
• Ettercap: excelente para ataques de MITM (Man-in-the-Middle). Pode interceptar e modificar tráfego em redes locais.
• dsniff: pacote com várias ferramentas de sniffing de senhas, incluindo captura de tráfego de protocolos como FTP, Telnet e HTTP.
