# 🛒 PDV Grêmio Estudantil - E.E. Profº João Teixeira Sampaio

Um sistema de Ponto de Venda (PDV) e gestão financeira desenvolvido especificamente para as operações diárias e eventos do Grêmio Estudantil. Construído para ser leve, rápido e totalmente independente.

## 🚀 Visão Geral
Este projeto foi desenhado para rodar diretamente no navegador e ser hospedado via **GitHub Pages**. A principal característica arquitetural é que o sistema roda **100% localmente no navegador** (via LocalStorage), sem qualquer comunicação ou armazenamento em bancos de dados em nuvem, como o Firebase. 

Isso garante que o sistema de carrinho e a área de administração funcionem sem atrasos, não gerem custos de servidor e possam operar mesmo com conexões de internet instáveis durante os intervalos da escola.

## ✨ Funcionalidades Principais
* **Frente de Caixa Rápida:** Interface visual para adicionar produtos ao carrinho, aplicar descontos e fechar vendas em poucos cliques.
* **Múltiplos Pagamentos:** Suporte para registros em Dinheiro e PIX (com campos para registrar nome e série do aluno).
* **Gestão de Cardápio:** Adição, edição e remoção de produtos e preços em tempo real.
* **Fechamento de Gaveta:** Interface dedicada para a contagem física de moedas e notas, cruzando automaticamente com o que foi registrado no sistema.
* **Relatórios e PDF:** Geração de relatórios de faturamento e impressão direta pelo navegador utilizando a biblioteca `html2pdf`.
* **Exportação de Dados:** Geração de planilhas CSV com o histórico completo de transações.
* **Sistema de Backups Local:** Ferramenta para exportar e importar todo o banco de dados do sistema em formato `.json`.
* **Personalização Visual:** Suporte a Modo Escuro/Claro, troca de cores de destaque e upload de logo através de arquivos locais.

## 🛠️ Tecnologias Utilizadas
* **HTML5, CSS3 & JavaScript (ES6+)**
* **React 18** (Executado via Babel Standalone / ES Modules)
* **TailwindCSS** (Estilização via CDN)
* **Lucide React** (Ícones da interface)

## ⚠️ Manutenção e Segurança de Dados
Devido à arquitetura focada em armazenamento local (LocalStorage), os dados ficam salvos apenas no dispositivo e navegador onde o PDV está sendo acessado. 

**Regra de Ouro:** É obrigatório utilizar a ferramenta de **Backup do Sistema** na aba "Configurações" após o fechamento de cada evento. Isso gera um arquivo `.json` que serve como proteção caso o cache do navegador da escola seja limpo.

---
*Desenvolvido por Thiago Pelegrineli Leal.*
