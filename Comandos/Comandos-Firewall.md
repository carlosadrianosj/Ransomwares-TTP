Este arquivo mantém comandos identificados que podem afetar o funcionamento do Firewall, cujos comandos são executados por ransomwares. 

**Utilizado para ativar a regra do Firewall que permite a descoberta de rede.**

"netsh.exe" advfirewall firewall set rule "group=”Network Discovery”" new enable=Yes


**Desativar completamente o Firewall do Windows, porém este comando se aplica a versões mais antigas do Windows, como o Windows XP e o Windows Server 2003.**

netsh firewall set opmode mode=disable

**Utilizado para desativar o firewall do Windows para o perfil de rede atualmente em uso. De modo geral, isso acaba por desligar o firewall para o perfil de rede específico que está atualmente ativo, como o público, particular ou de domínio. 
Este comando requer a utilização de privilégios para ser executado com sucesso.**


netsh advfirewall set currentprofile state off



