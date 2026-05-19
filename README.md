# 📅 Plataforma de Reserva de Recursos de Escritório

> Desafio de treinamento desenvolvido na **Stefanini** utilizando **Power Apps** e **Dataverse**.

---

## 📌 Sobre o Projeto

Solução desenvolvida para eliminar o uso de planilhas compartilhadas e trocas de e-mail no processo de agendamento de recursos corporativos. A plataforma centraliza e automatiza reservas de salas de reunião, projetores, vagas de estacionamento e estações de trabalho em uma interface intuitiva e integrada ao ecossistema Microsoft 365.

---

## ✅ Funcionalidades

- 📋 **Galeria de reservas agendadas** — visualização clara de todos os agendamentos ativos
- 🔍 **Filtro por tipo de recurso** — busca e filtragem por sala, projetor, vaga ou estação
- ➕ **Criação de reservas** — formulário completo com dados do recurso, data, horário e responsável
- ✏️ **Edição e exclusão de reservas** — gerenciamento total sobre agendamentos existentes
- 📧 **Notificação por e-mail** — envio automático de confirmação ao realizar uma reserva
- 📆 **Criação de evento no calendário** — integração com o calendário do usuário via Power Automate

---

## 🛠️ Tecnologias Utilizadas

| Tecnologia | Função |
|---|---|
| **Power Apps** | Interface da aplicação (canvas app) |
| **Dataverse** | Banco de dados e modelagem das entidades |
| **Conector de E-mail (Outlook)** | Envio de notificações e criação de eventos no calendário, via conexão nativa do Power Apps |
| **Microsoft 365** | Integração com Outlook e Calendar via conector nativo |

---

## 🗂️ Arquitetura da Solução

```
Power Apps (Canvas App)
    │
    ├── Tela de Galeria ──────────► Listagem e filtro de reservas
    ├── Tela de Criação ──────────► Formulário de nova reserva
    └── Tela de Edição/Exclusão ──► Gerenciamento de reservas
            │
            ▼
        Dataverse
    (Tabelas: Recursos, Reservas, Usuários)
            │
            ▼
  Conector Office 365 Outlook (nativo Power Apps)
    ├── Envio de e-mail de confirmação
    └── Criação de evento no calendário do usuário
```

---

## 💡 Problema Resolvido

Antes da solução, os colaboradores dependiam de:

- ❌ Planilhas compartilhadas sem controle de conflitos
- ❌ Trocas de e-mail manuais para solicitar recursos
- ❌ Falta de visibilidade sobre disponibilidade em tempo real

Com a plataforma:

- ✅ Reservas centralizadas em um único lugar
- ✅ Notificações automáticas sem intervenção manual
- ✅ Visibilidade em tempo real de todos os recursos

---

## 📸 Como Exportar e Importar no Power Apps

1. No [Power Apps](https://make.powerapps.com), acesse **Aplicativos**
2. Selecione o app e clique em **...** > **Exportar pacote**
3. Preencha as informações e baixe o arquivo `.zip`
4. Para importar: **Aplicativos** > **Importar tela** > faça upload do `.zip`

> ⚠️ Certifique-se de que o ambiente de destino possui o **Dataverse habilitado** e as mesmas conexões configuradas (Outlook, Calendar).

---

## 👤 Autor

Desenvolvido individualmente como desafio de treinamento na **Stefanini**.

---

## 📄 Licença

Este projeto foi desenvolvido para fins educacionais e de treinamento corporativo.
