# Endian Firewall 3.2.x





Lightsquid Report
=============

Addon para Endian Firewall 3.2, instalação rdo gerenciador de relatorios para Squid.



Versão:
--------

v.2.0 ( Testados no Endian Firewall Community nas versões 3.2.1, 3.2.2 e 3.2.4).



Requerimentos/opcional:
--------
- Requer: Acesso ao seu Endian Firewall atraves do console (Conexão SSH).



Instalando o Pacote:
--------

Realizando Download:

    curl -Lo lightsquid-endian3-2.0-1.x86_64.rpm https://raw.githubusercontent.com/brunoalmeida33/EndianFirewall3.2_Lightsquid/master/lightsquid-endian3-2.0-1.x86_64.rpm
    
    
Executando a instalação:

    rpm -Uvh lightsquid-endian3-2.0-1.x86_64.rpm
    
Definindo uma senha para o usuario lighsquid:

- Execute o script no console ssh: /usr/local/bin/lightsquid-password.sh ou lightsquid-password.sh. 
- Digite a senha a ser utilizada para acessar os relatorios e pressione ENTER.

Acesso direto aos relatorios:

Link: https://YOUENDIANGREENIP:10443/lightsquid   (Ex: https://192.168.0.15:10443/lightsquid )

Logue com o usuario lightsquid e forneça a senha configurada no passo anterior (scripts de senha).

Removendo o pacote:
--------
- No console ssh digite:

    rpm -e lightsquid-endian3
    
    
    
Outras informações:
------------------

- Esta instalação nao afeta o funcionamento dos relatorios nativo do Endian Firewall (SARG), não é necessario a remoção do mesmo.
- Para ativar este relatorio do lightsquid, é preciso selecionar a check box "Ativar Lightsquid" e clicar em "Salvar" no painel de controle do Endian, no menu  "Registros e relatorios" -> "Proxy" -> "Relatorio HTTP".
- Os relatorios serão gerados automaticamente a cada dia.

Espero ter ajudado.

Atenciosamente,

Bruno Almeida.
  
  
