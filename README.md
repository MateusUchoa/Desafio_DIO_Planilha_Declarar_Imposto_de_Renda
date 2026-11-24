# 📊 Organizador de Dados para Imposto de Renda (Excel)

Projeto desenvolvido como desafio prático da **DIO (Digital Innovation One)**. O objetivo é criar uma ferramenta no Microsoft Excel que funcione como um agregador de dados para organizar e validar as informações essenciais para a declaração do Imposto de Renda Pessoa Física (IRPF).

## 🎯 Funcionalidades Principais

- **Interface organizada em abas** para separação lógica das informações do contribuinte.
- **Validação de dados automática** com listas suspensas para evitar erros de preenchimento.
- **Cálculo automático de totais** nos informes de rendimentos bancários.
- **Base auxiliar de instituições financeiras** com códigos e nomes dos principais bancos brasileiros.
- **Controle de anexos** para rastrear os comprovantes em PDF de cada banco.

---

## 🗂️ Estrutura da Planilha

O arquivo `planilha_imposto_de_renda.xlsx` está dividido em **4 abas**:

| Aba | Descrição | Recursos Utilizados |
| :--- | :--- | :--- |
| **`TITULAR`** | Cadastro dos dados pessoais do contribuinte (Nome, CPF, Data de Nascimento, Título de Eleitor, Cônjuge, Endereço e Contatos). | Validação de dados (`SIM` / `NÃO`) |
| **`INFORMES`** | Registro dos informes de rendimentos por banco, valor atual e referência ao arquivo PDF de anexo. | Fórmula `=SOMA(D11;D16;D21)` e lista suspensa de bancos |
| **`NOTAS`** | Controle mensal de entradas financeiras (Data, Categoria e Valor). | Validação de dados (`HOLERITE`, `CNPJ`, `FREELANCE`) |
| **`TABELAS`** | Base de apoio com 50 bancos brasileiros (código + nome) usados nas validações. | Lista de referência para menus suspensos |

---

## 📸 Prévia do Projeto

*(Adicione aqui as capturas de tela salvas na pasta `/images`)*

- **Dados do Titular:** `<img width="973" height="483" alt="Captura de tela 2026-11-23 234059" src="https://github.com/user-attachments/assets/bae65646-7438-4158-a7e4-1ed0d79b8b36" />`
- **Informes Bancários:** `<img width="1069" height="479" alt="informes" src="https://github.com/user-attachments/assets/f74955b1-1fdc-42b1-a5c1-6689013303c7" />`
- **Notas e Entradas:** `<img width="1099" height="469" alt="notas" src="https://github.com/user-attachments/assets/c6428fe3-5fbb-4bdb-945b-85a96e062476" />`

---

## 🚀 Como Usar

1. Faça o download do arquivo `planilha_imposto_de_renda.xlsx` neste repositório.
2. Abra o arquivo no **Microsoft Excel**.
3. Preencha os dados cadastrais na aba **`TITULAR`**.
4. Cadastre seus bancos e saldos na aba **`INFORMES`** (o total será somado automaticamente).
5. Registre suas receitas mensais na aba **`NOTAS`** selecionando a categoria correta.

---

## 🛠️ Tecnologias e Conceitos Aplicados

- **Microsoft Excel** (Validação de Dados, Fórmulas de Soma, Estruturação de Tabelas Auxiliares e Navegação)
- **Git & GitHub** (Versionamento e Documentação Técnica em Markdown)
