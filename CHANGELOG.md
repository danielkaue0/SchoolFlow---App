
# 📋 Changelog - Controle Escolar

Todas as mudanças notáveis neste projeto serão documentadas neste arquivo.

O formato é baseado em [Keep a Changelog](https://keepachangelog.com/pt-BR/1.0.0/),
e este projeto adere ao [Versionamento Semântico](https://semver.org/lang/pt-BR/).

---

## [1.0.1] - Alpha - 2026-04-18

### ✨ Adicionado

#### 🎯 Sistema de Tarefas (CRUD Completo)
- Criar tarefas com título, descrição e prioridade
- Listar tarefas com scroll funcional
- Filtros: todas, pendentes, concluídas
- Editar tarefas existentes
- Excluir tarefas com confirmação
- Concluir/Reabrir tarefas
- Estatísticas em tempo real
- Armazenamento em JSON local

#### 📚 Sistema de Matérias
- Criar matérias com nome, professor e carga horária
- Listar matérias com scroll
- Adicionar horas de estudo
- Adicionar notas (0 a 10)
- Cálculo automático de média
- Status: Aprovado (≥7), Recuperação (5-6.9), Reprovado (<5)
- Barra de progresso de horas estudadas
- Estatísticas gerais
- Armazenamento em JSON local

#### 🍅 Pomodoro Timer
- Timer funcional com ciclo 25/5
- Controles: Iniciar, Pausar, Resetar
- Resetar ciclo atual ou resetar tudo
- Alternância automática entre trabalho e pausa
- Barra de progresso visual
- Notificação popup ao final do ciclo
- Thread separada para o timer (não trava a interface)
- Formato MM:SS

#### ⚙️ Configurações
- Tema claro/escuro (aplicação global)
- Ajuste de tempo do Pomodoro (trabalho e pausa)
- Ativar/desativar notificações
- Ativar/desativar sons
- Seleção de idioma (estrutura pronta)
- Resetar configurações para padrão
- Abas organizadas (Geral, Pomodoro, Aparência, Sobre)
- Armazenamento persistente em JSON

#### 🎨 Interface Gráfica (Tkinter)
- Navegação entre telas (Router pattern)
- Scroll em listas longas com suporte a mouse wheel
- Layout responsivo (redimensionável)
- Cards com informações
- Botões com efeito hover
- Diálogos modais para formulários
- Popup de confirmação ao sair (com teclas ESC/Enter)
- Logo automática ou personalizada

#### 🧩 Componentes Reutilizáveis
- Botão estilizado (Botao)
- Input de texto
- Lista de tarefas rolável (ListaTarefas)
- Item de tarefa individual (ItemTarefa)
- Timer widget (TimerWidget)
- Lista de matérias rolável (ListaMaterias)
- Item de matéria individual (ItemMateria)

#### 🛠️ Utilitários
- Gerenciador de tema (ThemeManager)
- Gerenciador de logo (LogoManager)
- Serviço de configurações (ConfigService)
- Serviço de tarefas (TarefaService)
- Serviço de matérias (MateriaService)
- Serviço de timer (TimerService)
- Estado global da aplicação (AppState)

#### 💾 Armazenamento
- Tarefas: `data/tarefas.json`
- Matérias: `data/materias.json`
- Configurações: `data/config/config.json`
- Persistência automática entre sessões

---

### 🐛 Corrigido

- Modo escuro agora é global (aplica em todas as telas)
- Responsividade ajustada (grid com weight)
- Scroll funcional em listas longas
- Timer não reseta ao pausar
- Popup de confirmação de saída funcionando
- Logo automática gerada programaticamente

---

### ⚠️ Problemas Conhecidos (Alpha)

- Caixas de diálogo podem perder foco (necessário Alt+Tab)
- Erro de callback em alguns casos (spam no console)
- Sistema de sons ainda não implementado
- Traduções apenas em português (estrutura pronta para EN)

---

## 📝 Como Contribuir

Envie os bugs encontrados e sugestões!

---

## 📞 Contato

- **Email**: controleescolarapp@gmail.com
- **GitHub**: https://github.com/danielkaue0