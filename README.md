# • Athom Studios | Recruitment

_Desenvolver um sistema de gestão de moradores, síndicos e condomínios utilizando Laravel_

## Bem-vindo(a)

Obrigado por participar do desafio da Athom Studios! Neste teste, você será responsável por desenvolver um sistema para uma rede de condomínios que gerencia os moradores, os síndicos e os próprios condomínios. O sistema deve atender às seguintes especificações e regras de negócio:

## Regras de Negócio:

- O sistema deve gerenciar os moradores, os síndicos e os condomínios.
- Cada morador deve estar vinculado a um apartamento dentro de um condomínio.
- Um síndico pode trabalhar em mais de um condomínio, mas apenas um síndico pode estar ativo por vez em um condomínio.
- Um morador pode ter apartamentos em vários condomínios ou ser removido de um condomínio.
- Apenas pessoas com permissões de síndico ou admin podem acessar o sistema.
- O usuário admin pode visualizar todos os dados do sistema, enquanto o síndico só tem acesso ao condomínio em que trabalha.

## Instruções

- Forke este repositório para sua conta pessoal do GitHub.
- Siga as especificações técnicas e de funcionalidade descritas abaixo.
- Ao concluir, envie o link do repositório para o e-mail mathuscardoso@gmail.com com o assunto Laravel Junior Developer Test.

## Especificações Técnicas

- Framework: Laravel 10
- Banco de Dados: MySQL ou PostgreSQL
- Versão do PHP: PHP 8.1
- Bootstrap: Utilizar o framework CSS Bootstrap para estilização básica.
- Autenticação: O sistema deve permitir que apenas síndicos e administradores façam login.
- Relacionamentos:
- - Moradores devem estar vinculados aos condomínios e apartamentos.
- - Síndicos podem gerenciar mais de um condomínio, mas um condomínio só pode ter um síndico ativo por vez.

## O que será avaliado?

- Arquitetura do projeto.
- Implementação das regras de negócio.
- Uso adequado do banco de dados.
- Clareza e organização do código.
- Utilização do Git e commits organizados.
- Documentação no README para configurar e executar o projeto.

## Funcionalidades

### Gerenciamento de Condomínios:

- Criar, editar e remover condomínios.
- Associar síndicos aos condomínios.
- Listar todos os condomínios da rede.

### Gerenciamento de Moradores:

- Adicionar, editar e remover moradores.
- Atribuir moradores a apartamentos dentro dos condomínios.
- Um morador pode ser associado a múltiplos condomínios e apartamentos.

### Gerenciamento de Síndicos:

- Adicionar e remover síndicos dos condomínios.
- Apenas um síndico pode estar ativo em um condomínio por vez.
- Um síndico pode trabalhar em mais de um condomínio, mas não ao mesmo tempo.

## Instruções para Compilar e Executar o Projeto

### Pré-requisitos:

- PHP 8.1+
- Composer
- MySQL ou PostgreSQL
- Laravel 10

## Passos:

1. Clone o repositório:

``` bash
git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio
```

2. Instale as dependências do projeto:

``` bash
composer install
```

3. Copie o arquivo .env.example para .env e configure suas variáveis de ambiente, como as credenciais do banco de dados:

``` bash
cp .env.example .env
```

4. Gere a chave da aplicação:

``` bash
php artisan key:generate
```

5. Execute as migrações para criar as tabelas no banco de dados:

``` bash
php artisan migrate
```

6. Inicie o servidor de desenvolvimento:

``` bash
php artisan serve
```

7. Acesse a aplicação no navegador:

``` bash
http://localhost:8000
```

### Testes Automatizados

Se aplicável, inclua testes automatizados para verificar as regras de negócio implementadas. Execute os testes com o seguinte comando:

``` bash
php artisan test
```
