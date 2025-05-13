# Universidade Federal do Tocantins, Câmpus Palmas 
### Curso: Bacharelado em Ciência da Computação
### Disciplina: Engenharia de Software
### Prof. Dr. Edeilson Milhomem da Silva

# Sistema de Gestão de Consultas Médicas

## Visão Geral
Sistema completo para gestão de consultas médicas, permitindo o cadastro de pacientes e agendamento eficiente de consultas. Ideal para clínicas e consultórios que precisam organizar seu fluxo de atendimento.

## Funcionalidades Principais

### Cadastro de Pacientes
- **Cadastro completo**: Registre pacientes com nome, telefone e e-mail
- **Gestão de dados**: Edite informações a qualquer momento
- **Controle total**: Remova pacientes quando necessário

### Agendamento de Consultas
- **Agendamentos completos**: Registre paciente, médico, data e hora em um único lugar
- **Visualização organizada**: Consulte todos os agendamentos por dia
- **Interface amigável**: Selecione horários disponíveis de forma intuitiva

### Visualização da Agenda
- **Visão diária completa**: Veja toda a agenda de consultas do dia
- **Filtros inteligentes**: Encontre consultas por médico ou especialidade
- **Disponibilidade clara**: Identifique horários livres e ocupados facilmente

  # Sprint Planning - CRUD de Agendamento Médico

## Objetivo da Sprint
Desenvolver as funcionalidades básicas de **CRUD (Create, Read, Update, Delete)** para:
 **Pacientes**  
 **Médicos**  
**Consultas**

---

## Tarefas (User Stories)

### 1. CRUD de Pacientes

#### US01 - Cadastrar Paciente
**Descrição**: Como administrador, quero cadastrar um novo paciente no sistema.  
**Critérios de Aceitação**:
- Campos obrigatórios: Nome, Telefone, E-mail, CPF
- Validação de CPF e e-mail
- Não permitir CPF duplicado

**Tarefas**:
- [ ] Criar formulário de cadastro
- [ ] Implementar validações
- [ ] Salvar no banco de dados

#### US02 - Editar Paciente
**Descrição**: Como administrador, quero editar informações de um paciente existente.  
**Critérios de Aceitação**:
- Carregar dados atuais no formulário
- Atualizar apenas campos modificados

**Tarefas**:
- [ ] Criar botão "Editar" na lista
- [ ] Implementar pré-carregamento do formulário

#### US03 - Excluir Paciente
**Descrição**: Como administrador, quero remover um paciente do sistema.  
**Critérios de Aceitação**:
- Exibir confirmação antes de excluir
- Impedir exclusão se houver consultas futuras

**Tarefas**:
- [ ] Criar botão "Excluir" com confirmação
- [ ] Verificar consultas agendadas

---

### 2. CRUD de Médicos

#### US04 - Cadastrar Médico
**Descrição**: Como administrador, quero cadastrar um novo médico.  
**Critérios de Aceitação**:
- Campos: Nome, CRM, Especialidade, Telefone
- Validação de CRM único

**Tarefas**:
- [ ] Criar formulário de cadastro
- [ ] Salvar no banco de dados

#### US05 - Listar Médicos
**Descrição**: Como usuário, quero ver uma lista de médicos disponíveis.  
**Critérios de Aceitação**:
- Exibir nome, especialidade e CRM
- Permitir filtro por especialidade

**Tarefas**:
- [ ] Criar tabela de médicos
- [ ] Implementar filtro

---

### 3. CRUD de Consultas

#### US06 - Agendar Consulta
**Descrição**: Como recepcionista, quero agendar uma consulta.  
**Critérios de Aceitação**:
- Selecionar paciente, médico, data e horário
- Não permitir agendamentos conflitantes

**Tarefas**:
- [ ] Criar formulário de agendamento
- [ ] Validar horários disponíveis

#### US07 - Cancelar Consulta
**Descrição**: Como recepcionista, quero cancelar uma consulta agendada.  
**Critérios de Aceitação**:
- Exibir confirmação
- Registrar motivo do cancelamento (opcional)

**Tarefas**:
- [ ] Criar botão "Cancelar"
- [ ] Implementar confirmação
