# BUSPÃ
Projeto-Buspa
🚌 Sistema de Transporte Universitário

Um sistema web completo para gerenciamento de transporte universitário, desenvolvido como projeto acadêmico.

📋 Descrição do Projeto

Sistema de transporte universitário que permite aos alunos visualizar rotas, consultar horários e fazer reservas de ônibus de forma simples e intuitiva.

✨ Funcionalidades

🔐 Sistema de Autenticação Cadastro de usuários com validação de email único

Login seguro com verificação de credenciais

Logout com redirecionamento automático

🗺️ Gestão de Transporte Visualização de rotas disponíveis

Consulta de horários por rota

Sistema de reservas integrado

Cancelamento de reservas ativas

👤 Área do Usuário Dashboard personalizado

Histórico de reservas

Status das reservas (ativa/cancelada)

🛠️ Tecnologias Utilizadas Frontend: HTML5, Tailwind CSS, JavaScript

Banco de Dados: SQL.js (SQLite no navegador)

Armazenamento: Local (navegador)

🚀 Como Executar o Projeto

Pré-requisitos Navegador web moderno

Editor de código (recomendado: VSCode)

Extensão Live Server (opcional)

Execução com VSCode Clone ou baixe o projeto

Abra o arquivo index.html no VSCode

Instale a extensão Live Server (se não tiver):

Vá em Extensions (Ctrl+Shift+X)

Procure por "Live Server" (Ritwick Dey)

Instale a extensão

Execute o projeto:

Clique com botão direito em index.html

Selecione "Open with Live Server"

Ou clique em "Go Live" no canto inferior direito

Execução Simples Abra diretamente o arquivo index.html no navegador

Ou arraste o arquivo para uma janela do navegador

📖 Como Usar o Sistema

Primeiro Acesso Inicie o sistema clicando em "Iniciar Sistema"

Cadastre-se ou use as credenciais de exemplo:

Email: admin@universidade.com

Senha: 123456

Navegando no Sistema Rotas: Visualize todas as rotas disponíveis

Horários: Consulte os horários por rota

Reservas: Faça e gerencie suas reservas

Fazendo uma Reserva Acesse a aba "Rotas"

Clique em "Ver Horários" na rota desejada

Selecione um horário e clique em "Fazer Reserva"

Confirme a reserva na aba "Minhas Reservas"

🗃️ Estrutura do Banco de Dados

O sistema utiliza 4 tabelas principais:

users - Usuários do sistema id (INTEGER, PRIMARY KEY)

email (TEXT, UNIQUE)

password (TEXT)

tipo (TEXT) - 'aluno' ou 'admin'

rotas - Rotas de transporte id (INTEGER, PRIMARY KEY)

nome (TEXT)

origem (TEXT)

destino (TEXT)

descricao (TEXT)

horarios - Horários das rotas id (INTEGER, PRIMARY KEY)

rota_id (INTEGER, FOREIGN KEY)

horario_saida (TEXT)

reservas - Reservas dos usuários id (INTEGER, PRIMARY KEY)

user_id (INTEGER, FOREIGN KEY)

rota_id (INTEGER, FOREIGN KEY)

horario_id (INTEGER, FOREIGN KEY)

data_reserva (TEXT)

status (TEXT) - 'ativa' ou 'cancelada'

🎯 Dados de Exemplo Incluídos

Rotas Pré-cadastradas Campus Central: Centro → Campus Universitário

Zona Norte: Zona Norte → Campus Universitário

Zona Sul: Zona Sul → Campus Universitário

Horários Disponíveis Múltiplos horários por rota (07:00, 08:30, 10:00, etc.)

Usuário Admin Email: admin@universidade.com

Senha: 123456

🔧 Características Técnicas

Frontend Design Responsivo com Tailwind CSS

Interface Dark Mode otimizada

Validação em tempo real de formulários

Feedback visual para todas as ações

Backend (Client-side) Banco SQLite no navegador com SQL.js

Persistência local durante a sessão

Consultas parametrizadas contra SQL injection

Transações ACID garantidas

📱 Compatibilidade

✅ Chrome 60+

✅ Firefox 55+

✅ Safari 11+

✅ Edge 79+

🐛 Solução de Problemas

Erro ao carregar banco de dados Solução: Recarregue a página e clique em "Iniciar Sistema"

Reserva não confirmada Solução: Verifique se já existe reserva ativa para o mesmo horário

Login não funciona Solução: Use as credenciais de exemplo ou cadastre novo usuário

📄 Licença

Este projeto foi desenvolvido para fins acadêmicos.

👨‍💻 Desenvolvido por

Projeto acadêmico - Sistema de Transporte Universitário