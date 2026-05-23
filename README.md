💊 FarmaFlux
Gestão de Fluxo de Caixa para Farmácias
Simples, rápido, gratuito para hospedar — com reconhecimento de voz e exportação Excel.
📌 Sobre o Projecto
O FarmaFlux é uma aplicação web desenvolvida especialmente para farmácias que precisam de registar e gerir o fluxo de caixa diário de forma eficiente, sem depender de sistemas caros e complexos.
Permite introduzir dados por voz ou manualmente, gerar planilhas Excel organizadas por dia ou por mês, controlar o acesso a downloads através de códigos de uso único, e manter uma base de dados de medicamentos e fornecedores.
✨ Funcionalidades
🎙 Reconhecimento de Voz
Ditado contínuo em Português (PT)
Comando "espaço" → passa para a próxima linha automaticamente
Comando "apagar" → remove a última linha registada
Comando "stop" → encerra a gravação
Funciona sem interrupções até ser parado
📋 Gestão de Projectos
Criar múltiplos fluxos de caixa (por dia, por turno, etc.)
Cabeçalho com nome da entidade, data e dia da semana gerado automaticamente
Colunas configuráveis: activar/desactivar Nº Ordem, Descrição e Valor
Todos os dados são guardados automaticamente na sessão
💰 Tabela de Registos
Numeração de ordem gerada automaticamente
Autocomplete de medicamentos ao digitar
Preenchimento automático do preço ao seleccionar um medicamento
Suporte a PVP (Preço de Venda ao Público) e PVF (Preço de Venda às Farmácias)
Opção de IVA 16% por linha (com cálculo automático) ou isenção
Total geral calculado em tempo real
🗃 Base de Dados
Fornecedores: nome, NUIT, telefone, email, endereço completo
Medicamentos: nome, PVP, PVF, indicação de IVA
⬇ Downloads e Controlo de Acesso
Exportação para Excel (.xlsx) com formatação profissional
Download de um único dia ou de todos os dias de um mês (várias abas no mesmo ficheiro)
Códigos de acesso únicos gerados pelo administrador — cada código só funciona uma vez
Utilizadores sem conta podem descarregar apenas com o código fornecido
🔐 Área de Administrador
Acesso protegido por senha
Geração de códigos de download por projecto ou por mês
Histórico de códigos (válidos / utilizados)
Eliminação de projectos
🚀 Como Instalar e Executar
Pré-requisitos
Node.js versão 18 ou superior
Git
1. Clonar o repositório
Bash
2. Instalar dependências
Bash
3. Executar em modo de desenvolvimento
Bash
Abrir no browser: http://localhost:5173
4. Gerar versão de produção
Bash
Os ficheiros finais ficam na pasta /dist prontos para publicar.
☁️ Deploy Gratuito
Opção A — Vercel (Recomendado, mais simples)
Criar conta gratuita em vercel.com
Clicar em "Add New Project"
Ligar ao repositório GitHub
Clicar em Deploy — fica online em menos de 2 minutos
URL gerado automaticamente (ex: farmaflux.vercel.app)
Opção B — GitHub Pages
No ficheiro vite.config.js, adicionar:
Js
Instalar o plugin de deploy:
Bash
Adicionar ao package.json:
Json
Executar:
Bash
Activar GitHub Pages nas definições do repositório → Branch: gh-pages
Opção C — Netlify
Criar conta em netlify.com
Arrastar a pasta /dist para o painel do Netlify
Pronto — URL imediato e gratuito
🛠 Estrutura do Projecto
Código
📦 Dependências Principais
Pacote
Versão
Uso
react
^18
Interface de utilizador
xlsx (SheetJS)
^0.18
Exportação para Excel
vite
^5
Servidor de desenvolvimento e build
🔧 Configuração Inicial
Alterar a senha de administrador
No ficheiro src/farmaflux.jsx, linha 1 da secção Admin:
Js
⚠️ Importante: Nunca partilhe a senha de administrador. Altere-a antes de publicar.
🎙 Guia Rápido de Uso por Voz
O que dizer
O que acontece
Nome do medicamento
Regista na coluna Descrição
Valor numérico
Regista na coluna Valor
"espaço"
Guarda a linha actual e passa para a próxima
"apagar"
Remove a última linha registada
"stop"
Encerra o reconhecimento de voz
Dica: Pode trabalhar só com valores dizendo números um a um e dando "espaço" entre cada um. A ordem é gerada automaticamente.
💡 Casos de Uso
Farmácia pequena ou média sem sistema de gestão
Registo de vendas diárias ao balcão
Controlo de entrada de mercadoria de fornecedores
Geração de relatório mensal para contabilidade
Partilha de ficheiros Excel com o gestor ou contabilista via código
🗺 Funcionalidades Futuras (Roadmap)
[ ] Autenticação de utilizadores com email e senha
[ ] Sincronização em nuvem (Firebase / Supabase)
[ ] Modo offline com sincronização automática
[ ] Relatórios gráficos (entradas vs saídas por mês)
[ ] Impressão directa de recibos
[ ] App móvel (Android / iOS) via React Native
[ ] Integração com leitores de código de barras
[ ] Multi-utilizador com perfis (caixa, gestor, contabilista)
🤝 Contribuições
Contribuições são bem-vindas! Para contribuir:
Fazer fork do repositório
Criar uma branch: git checkout -b minha-funcionalidade
Fazer commit: git commit -m 'Adiciona nova funcionalidade'
Push: git push origin minha-funcionalidade
Abrir um Pull Request
📄 Licença
Este projecto está sob licença MIT — pode usar, modificar e distribuir livremente, inclusive para fins comerciais.
👨‍💻 Créditos
Desenvolvido com ❤️ para tornar a gestão de farmácias mais acessível.
Interface construída com React + SheetJS + Web Speech API.
FarmaFlux — Porque a gestão da sua farmácia não deve custar uma fortuna.
