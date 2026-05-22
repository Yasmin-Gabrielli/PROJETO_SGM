# SGM - Sistema de Gestão de Manutenção

Este é um sistema web desenvolvido em PHP nativo para a gestão de chamados de manutenção corretiva, focado na organização por **Ambientes** (Blocos e Salas).

## 🚀 Funcionalidades

O sistema é dividido em três perfis de acesso:

*   **Solicitante:** Abre chamados enviando descrição e fotos, escolhendo o Bloco e o Ambiente.
*   **Técnico:** Visualiza sua agenda de tarefas, inicia a execução e reporta a solução.
*   **Gestor:** Realiza a triagem, define prioridades, atribui técnicos, gerencia usuários e ambientes, além de visualizar indicadores.

## 🛠️ Tecnologias Utilizadas

*   **Backend:** PHP (Nativo)
*   **Frontend:** HTML5, CSS3, Bootstrap 5
*   **Banco de Dados:** MySQL / MariaDB
*   **Ícones:** Phosphor Icons e Bootstrap Icons
*   **Comunicação:** AJAX (Fetch API) com retornos em JSON

## 📋 Pré-requisitos

Para rodar o projeto localmente, você precisará de um ambiente que suporte PHP e MySQL, como:
*   [XAMPP](https://www.apachefriends.org/index.html)
*   [WampServer](https://www.wampserver.com/)
*   [Laragon](https://laragon.org/)

**Versões recomendadas:**
*   PHP >= 7.4
*   MySQL >= 5.7

## 🔧 Instalação e Configuração

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/seu-usuario/PROJETO_SGM.git
    ```

2.  **Importe o Banco de Dados:**
    *   Abra o **phpMyAdmin** ou sua ferramenta SQL de preferência.
    *   Crie um banco de dados chamado `sgm_db`.
    *   Importe o arquivo SQL localizado em: `stand-by/BancoDeDados.sql`.

3.  **Configure a Conexão:**
    *   Abra o arquivo `config/database.php`.
    *   Ajuste as credenciais de `host`, `user` e `pass` de acordo com seu ambiente local.

4.  **Inicie o Servidor:**
    *   Coloque a pasta do projeto no `htdocs` (XAMPP) ou `www` (Wamp).
    *   Acesse no navegador: `http://localhost/PROJETO_SGM/login.php`.

## 🔐 Credenciais de Teste (Padrão)

| Perfil | E-mail | Senha |
| :--- | :--- | :--- |
| **Gestor** | admin@sgm.com | 123456 |
| **Técnico** | tecnico@sgm.com | 123456 |
| **Solicitante** | usuario@sgm.com | 123456 |

*Nota: As senhas no script SQL podem estar em hash. Para testes manuais, certifique-se de que o hash no banco corresponde à senha desejada.*

## 📂 Estrutura de Pastas

*   `/api`: Scripts PHP para processamento de dados e requisições AJAX.
*   `/assets`: Arquivos estáticos (CSS, JS, Imagens).
*   `/config`: Configurações de conexão com o banco de dados.
*   `/layout`: Componentes reutilizáveis (Header, Sidebar).
*   `/stand-by`: Documentação do projeto (User Stories, Casos de Uso e Script SQL).

---
Desenvolvido como parte do projeto de Gestão de Manutenção.