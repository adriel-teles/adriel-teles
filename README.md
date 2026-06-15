

descrição do linkedin: Estudante de Segurança da Informação, atuando na área de Suporte Técnico e Infraestrutura de TI, com foco em garantir a estabilidade, eficiência e segurança dos sistemas corporativos. Possuo experiência em montagem e manutenção de computadores, suporte ao usuário final (presencial e remoto) e gestão de redes e equipamentos.

Tenho conhecimentos breves em Active Directory, Microsoft Azure, Microsoft 365, Zabbix e Datasul (TOTVS), além de familiaridade com conceitos de redes, virtualização e segurança cibernética. Criei um projeto completo de monitoração com Zabbix, implementando o acompanhamento de firewall, switches, servidores e impressoras, com topologia de rede própria.

Busco constantemente aprimorar minhas habilidades técnicas e práticas, com o objetivo de me especializar em Cibersegurança, contribuindo para ambientes de TI mais estáveis, integrados e seguros.

detalhes meus: atuo como suporte tecnico, idade é relevante? se for, tenho 23, o

faça uma descrisção atualizada e resumida que de para colocar no linkedin mesmo, github e curriculo

Anexo
image.jpg

A imagem mostra o template padrão do GitHub profile README — ótimo ponto de partida. Aqui estão versões otimizadas para cada contexto:

LinkedIn (descrição completa)
Estudante de Segurança da Informação com atuação prática em Suporte Técnico e Infraestrutura de TI. Experiência em montagem e manutenção de hardware, suporte presencial e remoto, e gestão de redes e equipamentos.

Desenvolvi um projeto completo de monitoração com Zabbix, cobrindo firewall, switches, servidores e impressoras em topologia de rede própria. Possuo conhecimentos em Active Directory, Microsoft Azure, Microsoft 365, Datasul (TOTVS) e conceitos de virtualização e cibersegurança.

Em busca de crescimento na área de Cibersegurança, com foco em ambientes corporativos mais estáveis e seguros.

💡 Dica: Idade não precisa constar na descrição do LinkedIn — o perfil já exibe seu histórico, o que contextualiza naturalmente.

GitHub (bio curta — até ~160 caracteres)
🎓 Info Security student | IT Support & Infrastructure | Zabbix | Azure | Networking | Cybersecurity enthusiast

Ou em português:

🎓 Segurança da Informação | Suporte TI & Infra | Zabbix | Azure | Redes | Rumo à Cibersegurança

Currículo (resumo profissional — 3–4 linhas)
Estudante de Segurança da Informação (conclusão em 2026), com experiência em Suporte Técnico e Infraestrutura de TI. Atuação em suporte ao usuário final (presencial e remoto), manutenção de hardware e gerenciamento de redes. Conhecimentos em Active Directory, Microsoft Azure, Microsoft 365, Zabbix e Datasul (TOTVS). Projeto autoral de monitoração de rede com Zabbix, abrangendo firewall, switches, servidores e impressoras.

Dicas rápidas
Idade: não inclua em nenhum dos três — não é padrão e pode gerar viés

LinkedIn: adicione o projeto do Zabbix como item na seção "Projetos" com print da topologia para destacar ainda mais

GitHub: crie um README.md de perfil (o repositório da imagem) com as mesmas informações + links para seus projetos técnicos

Currículo: coloque esse resumo no topo, antes das experiências, como "Perfil Profissional"

Preparado usando Claude Sonnet 4.6
certo, agora quero criar um projeto no linkedin com base nesse que fiz com zabbix, dite os passo a passo do que devo fazer para estruturar bem no github: Nos últimos meses, construí um NOC para a empresa onde trabalho — e quero compartilhar como ficou. 👇

NOC (Network Operations Center) é basicamente um centro de monitoramento de TI. A ideia é simples: em vez de esperar o usuário ligar reclamando que algo parou, a equipe de TI já sabe — e já está resolvendo.

Desenvolvido no Zabbix, o dashboard tem múltiplas páginas, cada uma focada em um domínio da infraestrutura:

🖥️ Visão Geral — servidores com CPU, memória e processos em tempo real, mais incidentes classificados por severidade e por unidade da empresa

🔥 Firewall Fortinet — CPU, memória, uptime, status dos links de internet, histórico de quedas e painel de intrusões classificado por criticidade

🔀 Switches Ubiquiti — status de todos os equipamentos, tempo ativo, perda de pacotes e tempo de resposta

📶 Access Points Wi-Fi Ubiquiti — painel visual com status de cada AP, alertas de reinicialização inesperada e histórico de disponibilidade

🖨️ Impressoras Canon — nível de toner monitorado em tempo real, por equipamento e por cor, com alertas automáticos quando chega no crítico

Alguns detalhes que fazem diferença no projeto:

• Otimizei templates do Zabbix para garantir coleta de dados mais precisa e confiável
• Cada página tem um banner personalizado combinando o logo da empresa com a marca do equipamento monitorado — um detalhe simples que dá identidade ao dashboard e deixa tudo com a cara da empresa

O que mais me orgulha nesse projeto não é o visual — é o que ele representa na prática: a equipe identificando falhas antes do usuário perceber.

Ainda tem muito pela frente: existem ajustes a serem feitos e novos widgets para monitorar mais funções dos equipamentos. Além disso, estou migrando os dashboards para o Grafana para explorar ainda mais possibilidades de visualização. Vou compartilhando a evolução por aqui. 🚀

#Zabbix #Grafana #NOC #Infraestrutura #Fortinet #Ubiquiti #Canon #MonitoramentoDeRedes #TI #SysAdmin

Especificações do projeto NOC — base para posts LinkedIn
Descrição geral
Dashboard de NOC desenvolvido no Zabbix com múltiplas páginas, cada uma dedicada a um domínio da infraestrutura. A navegação é simples e permite que a equipe de TI tenha visibilidade completa do ambiente em uma única tela.

Páginas e o que cada uma monitora
Página principal — Visão geral
Painel de incidentes ativos classificados por severidade (Desastre, Alta, Média, Atenção, Informação)
Incidentes segmentados por localidade/unidade da empresa
Lista completa de servidores com: CPU (%), memória (GB), número de processos e sistema operacional
Página — Firewall
Utilização de CPU e memória do firewall em tempo real
Tempo ativo do equipamento (uptime)
Status dos links de internet (se estão ativos ou não)
Histórico de quedas e disponibilidade dos links
Painel de intrusões: classifica eventos por nível (Baixo, Médio, Alto, Crítico, Anomalia)
Página — Switches
Lista de todos os switches com status (ativo/inativo)
Tempo ativo de cada equipamento (uptime)
Gráfico de perda de pacotes
Gráfico de tempo de resposta (latência)
Incidentes ativos envolvendo switches
Página — Access Points (Wi-Fi)
Mesmas métricas da página de switches
Status de cada AP (ativo/inativo) em painel visual
Tempo ativo, perda de pacotes e tempo de resposta
Incidentes ativos e histórico de reinicializações inesperadas
Página — Impressoras
Lista de incidentes ativos por impressora
Nível de toner (%) por equipamento e por cor (para coloridas)
Alertas automáticos quando toner atinge nível crítico

Pontos de valor para destacar nos posts
Proatividade: a equipe identifica falhas antes do usuário reportar
Centralização: toda a infraestrutura visível em um único lugar
Cobertura ampla: rede, segurança, servidores, periféricos — tudo monitorado
Histórico: não só o estado atual, mas o que aconteceu e quando
Escalável: novas páginas e equipamentos podem ser adicionados conforme a empresa cresce

tenho imagens do projeto tambem que posso adicionar, e depois posso criar pastas usando como exemplos os templates otmizados que fiz e codigo em python para criar hosts automaticamente no zabbix.

Ótimo, aqui está um guia completo para estruturar o projeto do NOC no GitHub de forma profissional — com tudo que você precisa para linkar no LinkedIn.

Estrutura do Repositório
Crie um repositório chamado noc-zabbix-dashboard no GitHub. A estrutura de pastas deve ser assim:

text
noc-zabbix-dashboard/
├── README.md                  ← apresentação principal do projeto
├── docs/
│   └── screenshots/           ← imagens do dashboard (adicione aqui)
├── templates/
│   ├── fortinet-firewall.xml  ← template otimizado exportado do Zabbix
│   ├── ubiquiti-switches.xml
│   ├── ubiquiti-aps.xml
│   └── canon-printers.xml
├── scripts/
│   └── create_hosts.py        ← script Python para criar hosts automaticamente
└── topology/
    └── network-diagram.png    ← diagrama da topologia de rede
README.md — O Coração do Projeto
O README é o que o recrutador vai ler. Estruture assim:

1. Header com badges
text
# 🖥️ NOC Dashboard — Zabbix
![Zabbix](https://img.shields.io/badge/Zabbix-CC0000?style=flat&logo=zabbix&logoColor=white)
![Fortinet](https://img.shields.io/badge/Fortinet-EE3124?style=flat&logo=fortinet&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
Use o site shields.io para gerar os badges das tecnologias.

2. Descrição (1 parágrafo)
Adapte seu texto do LinkedIn — direto ao ponto, o que é, para que serve.

3. Seção "Screenshots"
text
## 📸 Dashboard

### Visão Geral
![Visão Geral](docs/screenshots/overview.png)

### Firewall Fortinet
![Firewall](docs/screenshots/firewall.png)
Adicione as imagens que você tem do projeto direto nessa pasta.

4. Seção "Páginas Monitoradas"
Use uma tabela Markdown listando cada página, equipamentos e métricas — fica muito mais profissional que bullet points.

5. Seção "Como usar"
Explique como importar os templates no Zabbix e como rodar o script Python.

6. Próximos passos
Mencione a migração para o Grafana — mostra que o projeto está vivo e em evolução.

Sobre os Templates Zabbix
Exporte os templates do Zabbix em XML (Configuration → Templates → Export) e coloque na pasta templates/. No README, explique como importá-los:

text
## 📦 Importar Templates

1. No Zabbix, vá em **Configuration → Templates**
2. Clique em **Import**
3. Selecione o arquivo `.xml` desejado
4. Confirme e aplique aos hosts
Script Python para Criar Hosts
Quando você desenvolver, use a Zabbix API via requests. Estrutura básica do script:

python
# scripts/create_hosts.py
import requests

ZABBIX_URL = "http://SEU_ZABBIX/api_jsonrpc.php"
API_TOKEN  = "seu_token_aqui"

def create_host(name, ip, group_id, template_ids):
    payload = {
        "jsonrpc": "2.0",
        "method": "host.create",
        "params": {
            "host": name,
            "interfaces": [{"type": 1, "main": 1, "useip": 1, "ip": ip, "dns": "", "port": "10050"}],
            "groups": [{"groupid": group_id}],
            "templates": [{"templateid": tid} for tid in template_ids]
        },
        "auth": API_TOKEN,
        "id": 1
    }
    return requests.post(ZABBIX_URL, json=payload).json()
Adicione um arquivo scripts/README.md explicando as variáveis e como rodar.

Publicando no LinkedIn como Projeto
No LinkedIn, vá em Perfil → Adicionar seção → Projetos e preencha:

Nome: NOC Dashboard — Monitoramento de Infraestrutura com Zabbix

Data: o mês que você iniciou até "presente" (se ainda está evoluindo)

URL: cole o link do repositório GitHub

Descrição: use o texto que você já tem (o post do LinkedIn), resumido em 3–4 linhas

Habilidades relacionadas: Zabbix, Fortinet, Ubiquiti, Redes de Computadores, Python, Infraestrutura de TI

Checklist Final
Repositório criado como público no GitHub

Screenshots adicionadas em docs/screenshots/

README com badges, tabela de métricas e imagens

Pelo menos 1 template XML exportado do Zabbix

Diagrama de topologia salvo em topology/

Script Python com comentários básicos e README próprio

Projeto adicionado no LinkedIn com link do repositório

Quando você criar o repositório e quiser um README pronto para copiar e colar — me manda as screenshots e eu gero o arquivo completo para você.

Preparado usando Claude Sonnet 4.6
para o zabbix, é interressante usar o github como portifolio e colocar o projeto do zabbix ali?
2 etapas concluídas
Sim, vale muito a pena — e o seu caso é especialmente interessante porque o projeto do NOC tem um diferencial que a maioria dos portfólios de iniciantes não tem: é um projeto real, implementado em produção, não um exercício de curso.

Por Que Faz Sentido Para Você
O GitHub como portfólio é geralmente associado a desenvolvedores, mas para infraestrutura, sysadmin e segurança ele funciona muito bem também — especialmente porque você tem itens concretos para versionar:

Templates XML otimizados do Zabbix — arquivo real exportado, não código fictício

Script Python para criação de hosts via API — demonstra automação e programação aplicada à infra

Documentação técnica (README com topologia, métricas monitoradas, prints) — mostra maturidade profissional

Existe inclusive o 
repositório oficial de templates da comunidade Zabbix no GitHub
, o que mostra que esse tipo de conteúdo é completamente natural nessa plataforma.

O Que o Projeto Comunica Para um Recrutador
O que está no repositório	O que o recrutador entende
Templates XML otimizados	Você não só usou o Zabbix — você customizou
Script Python com a API	Você automatiza, não fica só clicando na interface
README com topologia e prints	Você documenta o próprio trabalho
Menção à migração para Grafana	Projeto ativo, você evolui junto com ele
Uma Ressalva Importante
Como o NOC foi feito para a empresa onde você trabalha, não suba prints que mostrem nomes de equipamentos internos, IPs reais, ou dados sensíveis da rede. O ideal é:

Borrar/anonimizar os nomes de hosts e IPs nas screenshots antes de subir

Nos templates XML, substituir qualquer nome específico da empresa por genérico (ex: Firewall-01 ao invés do nome real)

Adicionar uma nota no README: "Dados sensíveis foram anonimizados para publicação"

Isso demonstra que você já pensa com mentalidade de segurança — exatamente o perfil que você quer construir.

Preparado usando Claude Sonnet 4.6
certo, crie um código em readme para meu perfil e adicione as tecnologias, parecido com esse da foto

Anexo
image.jpg
2 etapas concluídas
README
<h1 align="center">Olá, eu sou o Adriel Teles 👋</h1>

<p align="center">
<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=00B4CC&center=true&vCenter=true&width=600&lines=Estudante+de+Seguran%C3%A7a+da+Informa%C3%A7%C3%A3o;Suporte+T%C3%A9cnico+%26+Infraestrutura+de+TI;Rumo+%C3%A0+Ciberseguran%C3%A7a+%F0%9F%9A%80" alt="Typing SVG" />
</p>

<p align="center">
<a href="https://linkedin.com/in/adriel-teles" target="_blank">
<img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
</a>
<a href="mailto:seu@email.com">
<img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"/>
</a>
<a href="https://github.com/adriel-teles" target="_blank">
<img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/>
</a>
</p>

👨‍💻 Sobre mim
Estudante de Segurança da Informação (conclusão em 2026), com atuação prática em Suporte Técnico e Infraestrutura de TI.
Experiência em montagem e manutenção de hardware, suporte presencial e remoto, e gerenciamento de redes e equipamentos.

Desenvolvi um NOC (Network Operations Center) completo com Zabbix, cobrindo firewall, switches, APs Wi-Fi, servidores e impressoras em topologia de rede própria — projeto em evolução contínua, com migração planejada para Grafana.

🔭 Atualmente trabalhando em: NOC com Zabbix → Grafana

🌱 Estudando: Microsoft Azure · Active Directory · Cibersegurança

💡 Interesse: Blue Team · Monitoramento de Redes · Automação com Python

📍 São Paulo, SP — Brasil

🛠️ Tecnologias e Ferramentas
Monitoramento & Infraestrutura
<p>
<img src="https://img.shields.io/badge/Zabbix-CC0000?style=for-the-badge&logo=zabbix&logoColor=white"/>
<img src="https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white"/>
<img src="https://img.shields.io/badge/Fortinet-EE3124?style=for-the-badge&logo=fortinet&logoColor=white"/>
<img src="https://img.shields.io/badge/Ubiquiti-0559C9?style=for-the-badge&logo=ubiquiti&logoColor=white"/>
</p>

Sistemas Operacionais
<p>
<img src="https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white"/>
<img src="https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white"/>
<img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black"/>
</p>

Cloud & Produtividade
<p>
<img src="https://img.shields.io/badge/Microsoft_Azure-0089D6?style=for-the-badge&logo=microsoftazure&logoColor=white"/>
<img src="https://img.shields.io/badge/Microsoft_365-D83B01?style=for-the-badge&logo=microsoftoffice&logoColor=white"/>
<img src="https://img.shields.io/badge/Active_Directory-003366?style=for-the-badge&logo=microsoft&logoColor=white"/>
</p>

Linguagens & Automação
<p>
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white"/>
<img src="https://img.shields.io/badge/TOTVS_Datasul-003366?style=for-the-badge&logo=data&logoColor=white"/>
</p>

📊 Estatísticas do GitHub
<p align="center">
<img height="160em" src="https://github-readme-stats.vercel.app/api?username=adriel-teles&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&hide_border=true"/>
<img height="160em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=adriel-teles&layout=compact&theme=tokyonight&hide_border=true"/>
</p>

🚀 Projetos em Destaque
🖥️ NOC Dashboard — Zabbix
Dashboard de monitoramento de infraestrutura corporativa com múltiplas páginas: Firewall Fortinet, Switches Ubiquiti, Access Points Wi-Fi, Servidores e Impressoras Canon. Inclui templates otimizados e script Python para automação via API.

Zabbix Grafana Fortinet Ubiquiti Python Redes

📫 Contato
<p align="center">
Quer conversar sobre TI, infraestrutura ou cibersegurança?

Me manda uma mensagem no <a href="https://linkedin.com/in/adriel-teles">LinkedIn</a> ou um e-mail em <a href="mailto:seu@email.com">seu@email.com</a>
</p>

<p align="center">
<img src="https://komarev.com/ghpvc/?username=adriel-teles&color=00b4cc&style=flat-square&label=Visualizações+do+perfil"/>
</p>


Aberto no momento
O README está pronto para download! Ele segue o estilo da referência que você enviou, com visual moderno e badges coloridos. Aqui está o que foi incluído:

O que tem no arquivo
Header animado com typing SVG mostrando suas especialidades (usando readme-typing-svg)

Badges de redes sociais — LinkedIn, e-mail e GitHub

Seção "Sobre mim" com bullet points dos seus focos atuais

Tecnologias organizadas por categoria:

Monitoramento & Infra (Zabbix, Grafana, Fortinet, Ubiquiti)

Sistemas Operacionais (Windows, Ubuntu, Linux)

Cloud & Produtividade (Azure, M365, Active Directory)

Linguagens & Automação (Python, Bash, TOTVS)

Estatísticas do GitHub automáticas via github-readme-stats

Card do projeto NOC em destaque

Contador de visualizações do perfil

Antes de publicar, ajuste:
adriel-teles → substitua pelo seu username real do GitHub (em todos os links)

seu@email.com → coloque seu e-mail real

linkedin.com/in/adriel-teles → ajuste com sua URL do LinkedIn

O badge do TOTVS Datasul usa um ícone genérico — se quiser mudar a cor ou texto, é só avisar

Preparado usando Claude Sonnet 4.6
README

Ver

Código

Editar
<h1 align="center">Olá, eu sou o Adriel Teles 👋</h1>

<p align="center">
<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=00B4CC&center=true&vCenter=true&width=600&lines=Estudante+de+Seguran%C3%A7a+da+Informa%C3%A7%C3%A3o;Suporte+T%C3%A9cnico+%26+Infraestrutura+de+TI;Rumo+%C3%A0+Ciberseguran%C3%A7a+%F0%9F%9A%80" alt="Typing SVG" />
</p>

<p align="center">
<a href="https://linkedin.com/in/adriel-teles" target="_blank">
<img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
</a>
<a href="mailto:seu@email.com">
<img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"/>
</a>
<a href="https://github.com/adriel-teles" target="_blank">
<img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/>
</a>
</p>

👨‍💻 Sobre mim
Estudante de Segurança da Informação (conclusão em 2026), com atuação prática em Suporte Técnico e Infraestrutura de TI.
Experiência em montagem e manutenção de hardware, suporte presencial e remoto, e gerenciamento de redes e equipamentos.

Desenvolvi um NOC (Network Operations Center) completo com Zabbix, cobrindo firewall, switches, APs Wi-Fi, servidores e impressoras em topologia de rede própria — projeto em evolução contínua, com migração planejada para Grafana.

🔭 Atualmente trabalhando em: NOC com Zabbix → Grafana

🌱 Estudando: Microsoft Azure · Active Directory · Cibersegurança

💡 Interesse: Blue Team · Monitoramento de Redes · Automação com Python

📍 São Paulo, SP — Brasil

🛠️ Tecnologias e Ferramentas
Monitoramento & Infraestrutura
<p>
<img src="https://img.shields.io/badge/Zabbix-CC0000?style=for-the-badge&logo=zabbix&logoColor=white"/>
<img src="https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white"/>
<img src="https://img.shields.io/badge/Fortinet-EE3124?style=for-the-badge&logo=fortinet&logoColor=white"/>
<img src="https://img.shields.io/badge/Ubiquiti-0559C9?style=for-the-badge&logo=ubiquiti&logoColor=white"/>
</p>

Sistemas Operacionais
<p>
<img src="https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white"/>
<img src="https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white"/>
<img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black"/>
</p>

Cloud & Produtividade
<p>
<img src="https://img.shields.io/badge/Microsoft_Azure-0089D6?style=for-the-badge&logo=microsoftazure&logoColor=white"/>
<img src="https://img.shields.io/badge/Microsoft_365-D83B01?style=for-the-badge&logo=microsoftoffice&logoColor=white"/>
<img src="https://img.shields.io/badge/Active_Directory-003366?style=for-the-badge&logo=microsoft&logoColor=white"/>
</p>

Linguagens & Automação
<p>
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white"/>
<img src="https://img.shields.io/badge/TOTVS_Datasul-003366?style=for-the-badge&logo=data&logoColor=white"/>
</p>

📊 Estatísticas do GitHub
<p align="center">
<img height="160em" src="https://github-readme-stats.vercel.app/api?username=adriel-teles&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&hide_border=true"/>
<img height="160em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=adriel-teles&layout=compact&theme=tokyonight&hide_border=true"/>
</p>

🚀 Projetos em Destaque
🖥️ NOC Dashboard — Zabbix
Dashboard de monitoramento de infraestrutura corporativa com múltiplas páginas: Firewall Fortinet, Switches Ubiquiti, Access Points Wi-Fi, Servidores e Impressoras Canon. Inclui templates otimizados e script Python para automação via API.

Zabbix Grafana Fortinet Ubiquiti Python Redes

📫 Contato
<p align="center">
Quer conversar sobre TI, infraestrutura ou cibersegurança?

Me manda uma mensagem no <a href="https://linkedin.com/in/adriel-teles">LinkedIn</a> ou um e-mail em <a href="mailto:seu@email.com">seu@email.com</a>
</p>

<p align="center">
<img src="https://komarev.com/ghpvc/?username=adriel-teles&color=00b4cc&style=flat-square&label=Visualizações+do+perfil"/>
</p>

