# HackFlow
 
Sistema de apoio à organização do 1º Hackathon do curso de Ciência da Computação — IFPR, Campus Pinhais.
 
Projeto Integrador da disciplina de **Engenharia de Software I** (Profa. Lauriana Paludo — turma BCC.2).
 
> Status atual: **Sprint 0 — Descoberta concluída.** Elicitação de requisitos e prototipação em andamento (Semanas 3–6).

Link do prototipo: https://app.quant-ux.com/#/test.html?h=a2aa10akv5D7oEZYsGucCqkJa3ENuIDONW07ug3gZgKCszcyp3fimlUdWOqy&ln=en
 
## Equipe
 
- Enzo Leonardo Ferreira Gonçalves
- Evellin Silva Sebastião
- Henrique Gabriel da Silva
- Kauã Vinicius Silva Alves
## Contexto
 
O campus está organizando seu 1º Hackathon institucional e ainda não possui um sistema próprio para apoiar o evento. Hoje, inscrição, submissão de projetos, avaliação dos jurados e divulgação de resultados dependem de planilhas e comunicação manual (e-mail/WhatsApp), o que já gerou:
 
- Inscrições duplicadas
- Informações desencontradas entre participantes e comissão
- Falta de um canal único de avisos durante o evento
- Avaliação dos jurados em papel, com apuração final demorada
## Stakeholder
 
**Comissão organizadora do Hackathon** — formada por uma professora, um monitor da disciplina de ESI e dois representantes do projeto de extensão Azure DevOps do IFPR. Atua como cliente do sistema: planeja, comunica e conduz o evento do início ao fim, mas não tem formação técnica nem tempo disponível para desenvolver ferramentas próprias.
 
**Outros públicos afetados:** equipes participantes do Hackathon, jurados, coordenação do curso e o público/comunidade acadêmica que acompanha o evento.
 
## Restrições
 
- **Orçamento:** zero para ferramentas pagas — o sistema é construído pela própria turma
- **Prazo:** funcional até a Semana 19, para uso real no evento na Semana 20
- **Simplicidade:** a comissão organizadora tem pouco tempo para aprender a operar o sistema
- **LGPD:** o sistema trata dados pessoais de participantes e deve fazer isso com cuidado
- **Usuários majoritariamente não técnicos**, o que exige interface simples e direta
## Escopo mínimo viável (primeira versão)
 
1. **Cadastro de equipes/participantes** com validação automática de inscrição (detecção de e-mail/CPF duplicado, edição centralizada do próprio cadastro)
2. **Submissão de projeto** pela equipe (link do repositório/arquivo + descrição), vinculada ao cadastro validado
3. **Painel de avaliação para jurados**, com nota por critério definido pela comissão
4. **Placar público (scoreboard)** com o andamento e o resultado das avaliações
5. **Central de avisos**, com alertas automáticos e centralizados sobre mudanças do evento, visíveis a todos os usuários cadastrados
### Fora do escopo desta entrega
 
- Pagamento ou qualquer cobrança dentro do sistema
- Chat ou mensageria interna entre equipes, jurados e comissão
- Aplicativo mobile nativo (a primeira versão é um site responsivo)
- Notificações push nativas (os avisos ficam concentrados na central de avisos)
- Matching automático de jurados por área de expertise
- Integração com redes sociais
## Backlog inicial (épicos)
 
1. Cadastro e autenticação de usuários (participante, jurado, admin)
2. Validação automática de inscrição (bloqueio/alerta de duplicidade + edição centralizada)
3. Submissão de projetos pelas equipes
4. Painel de avaliação dos jurados
5. Placar público (scoreboard) de resultados
6. Central de avisos e alertas do evento
7. Painel administrativo da comissão organizadora
## Processo de desenvolvimento
 
- **Framework:** Kanban, com fluxo contínuo (sem Sprints fixas)
- **Cerimônias:** alinhamento rápido às segundas e quintas-feiras; revisão semanal do quadro às sextas-feiras, para avaliar gargalos e ajustar limites de WIP
- **Quadro:** [GitHub Projects](https://github.com/features/issues), vinculado ao repositório do time, com colunas:
  `Backlog → A Fazer (WIP 3) → Em Progresso (WIP 2) → Em Revisão (WIP 2) → Concluído`
**Por que Kanban:** o projeto se encaixa como *Complicado tendendo a Complexo* no framework Cynefin — a tecnologia envolvida (cadastro, validação de dados, formulários web, painel de avaliação) é bem conhecida pela equipe, mas os requisitos ainda estão evoluindo (a comissão já trouxe duas necessidades novas na Semana 5: validação automática de inscrição e central de avisos). O Kanban absorve pedidos novos a qualquer momento, sem depender do fim de um ciclo fechado — diferente de Sprints fixas ou de um modelo em cascata.
 
## Próximos passos
 
- **Semana 6:** elicitar requisitos detalhados junto à comissão, a partir deste backlog inicial
- Quebrar os épicos em user stories menores dentro do GitHub Projects
- Confirmar critérios de aceite para a validação automática de inscrição e para a central de avisos
## Disciplina
 
Engenharia de Software I — Ciência da Computação, IFPR Campus Pinhais
Profa. Lauriana Paludo · Turma BCC.2
