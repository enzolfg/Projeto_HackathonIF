<div align="center">

# 🚀 HackFlow

**Sistema de apoio à organização do 1º Hackathon do curso**
Ciência da Computação — IFPR, Campus Pinhais

![Status](https://img.shields.io/badge/status-Sprint%200%20conclu%C3%ADda-A6721E?style=for-the-badge)
![Metodologia](https://img.shields.io/badge/metodologia-Kanban-2F6F68?style=for-the-badge)
![Disciplina](https://img.shields.io/badge/engenharia%20de%20software-I-14213D?style=for-the-badge)

[🎨 Ver protótipo da interface](https://app.quant-ux.com/#/test.html?h=a2aa10akv5D7oEZYsGucCqkJa3ENuIDONW07ug3gZgKCszcyp3fimlUdWOqy&ln=en) · [📋 Backlog](#️-backlog-inicial) · [🔄 Processo](#-processo-de-desenvolvimento)

</div>

---

## 📑 Sumário

- [Equipe](#-equipe)
- [Contexto](#-contexto)
- [Stakeholder](#-stakeholder)
- [Restrições](#️-restrições)
- [Protótipo de interface](#-protótipo-de-interface-gui)
- [Escopo mínimo viável](#-escopo-mínimo-viável-primeira-versão)
- [Fora do escopo](#-fora-do-escopo-desta-entrega)
- [Backlog inicial](#️-backlog-inicial)
- [Processo de desenvolvimento](#-processo-de-desenvolvimento)
- [Próximos passos](#️-próximos-passos)

---

## 👥 Equipe

| Integrante |
|---|
| Enzo Leonardo Ferreira Gonçalves |
| Evellin Silva Sebastião |
| Henrique Gabriel da Silva |
| Kauã Vinicius Silva Alves |

---

## 📌 Contexto

O campus está organizando seu 1º Hackathon institucional e ainda não possui um sistema próprio para apoiar o evento. Hoje, inscrição, submissão de projetos, avaliação dos jurados e divulgação de resultados dependem de planilhas e comunicação manual (e-mail/WhatsApp), o que já gerou:

- 🔁 Inscrições duplicadas
- ❗ Informações desencontradas entre participantes e comissão
- 📢 Falta de um canal único de avisos durante o evento
- 🐢 Avaliação dos jurados em papel, com apuração final demorada

---

## 🎯 Stakeholder

**Comissão organizadora do Hackathon** — uma professora, um monitor da disciplina de ESI e dois representantes do projeto de extensão Azure DevOps do IFPR. Atua como cliente do sistema: planeja, comunica e conduz o evento do início ao fim, mas não tem formação técnica nem tempo disponível para desenvolver ferramentas próprias.

> **Outros públicos afetados:** equipes participantes do Hackathon, jurados, coordenação do curso e o público/comunidade acadêmica que acompanha o evento.

---

## ⚠️ Restrições

| Restrição | Detalhe |
|---|---|
| 💰 Orçamento | Zero para ferramentas pagas — o sistema é construído pela própria turma |
| ⏳ Prazo | Funcional até a Semana 19, para uso real no evento na Semana 20 |
| 🧩 Simplicidade | A comissão tem pouco tempo para aprender a operar o sistema |
| 🔒 LGPD | O sistema trata dados pessoais de participantes e deve fazer isso com cuidado |
| 👤 Usuários | Majoritariamente não técnicos — exige interface simples e direta |

---

## 🖼️ Protótipo de interface (GUI)

O protótipo navegável da interface foi desenvolvido no Quant-UX e pode ser acessado no link abaixo:

<div align="center">

### [🎨 Abrir protótipo interativo →](https://app.quant-ux.com/#/test.html?h=a2aa10akv5D7oEZYsGucCqkJa3ENuIDONW07ug3gZgKCszcyp3fimlUdWOqy&ln=en)

</div>

---

## ✅ Escopo mínimo viável (primeira versão)

1. **Cadastro de equipes/participantes** com validação automática de inscrição (detecção de e-mail/CPF duplicado, edição centralizada do próprio cadastro)
2. **Submissão de projeto** pela equipe (link do repositório/arquivo + descrição), vinculada ao cadastro validado
3. **Painel de avaliação para jurados**, com nota por critério definido pela comissão
4. **Placar público (scoreboard)** com o andamento e o resultado das avaliações
5. **Central de avisos**, com alertas automáticos e centralizados sobre mudanças do evento, visíveis a todos os usuários cadastrados

## 🚫 Fora do escopo desta entrega

- Pagamento ou qualquer cobrança dentro do sistema
- Chat ou mensageria interna entre equipes, jurados e comissão
- Aplicativo mobile nativo (a primeira versão é um site responsivo)
- Notificações push nativas (os avisos ficam concentrados na central de avisos)
- Matching automático de jurados por área de expertise
- Integração com redes sociais

---

## 🗂️ Backlog inicial

<details open>
<summary><strong>Ver épicos do backlog</strong></summary>

1. Cadastro e autenticação de usuários (participante, jurado, admin)
2. Validação automática de inscrição (bloqueio/alerta de duplicidade + edição centralizada)
3. Submissão de projetos pelas equipes
4. Painel de avaliação dos jurados
5. Placar público (scoreboard) de resultados
6. Central de avisos e alertas do evento
7. Painel administrativo da comissão organizadora

</details>

---

## 🔄 Processo de desenvolvimento

- **Framework:** Kanban, com fluxo contínuo (sem Sprints fixas)
- **Cerimônias:** alinhamento rápido às segundas e quintas-feiras; revisão semanal do quadro às sextas-feiras, para avaliar gargalos e ajustar limites de WIP
- **Quadro:** GitHub Projects, vinculado ao repositório do time:

  `Backlog → A Fazer (WIP 3) → Em Progresso (WIP 2) → Em Revisão (WIP 2) → Concluído`

> **Por que Kanban?** O projeto se encaixa como *Complicado tendendo a Complexo* no framework Cynefin — a tecnologia envolvida (cadastro, validação de dados, formulários web, painel de avaliação) é bem conhecida pela equipe, mas os requisitos ainda estão evoluindo (a comissão já trouxe duas necessidades novas na Semana 5: validação automática de inscrição e central de avisos). O Kanban absorve pedidos novos a qualquer momento, sem depender do fim de um ciclo fechado — diferente de Sprints fixas ou de um modelo em cascata.

---

## ⏭️ Próximos passos

- [ ] **Semana 6:** elicitar requisitos detalhados junto à comissão, a partir deste backlog inicial
- [ ] Quebrar os épicos em user stories menores dentro do GitHub Projects
- [ ] Confirmar critérios de aceite para a validação automática de inscrição e para a central de avisos

---

<div align="center">

**Engenharia de Software I** · Ciência da Computação · IFPR Campus Pinhais
Profa. Lauriana Paludo · Turma BCC.2

</div>
