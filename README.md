# 🤠 O QUE EU ESTUDARIA SE FOSSE APRENDER PHP (E WEB EM GERAL) EM 2022

Primeiro eu acho importante estabelecer alguns conceitos básicos na mente.

## 🌎 Como funciona a internet?

Nesse ponto o que eu quero entender é o que acontece quando eu acesso uma URL.

- O que é HTTP?
- O que é arquitetura cliente e servidor?
- O que compõe uma mensagem HTTP?
- O que é um "request" HTTP e como isso se relaciona aos outros tópicos?
- O que é uma resposta HTTP?
- Verbos HTTP (GET, POST, PUT, DELETE)
- Códigos HTTP

É necessário entender um pouco sobre esses conceitos porque eles são muito úteis quando trabalhamos com tecnologias web. Boa parte do trabalho é seguir o request pelo código e devolver uma resposta apropriada.

## 🛑 Caminhos

Estude um pouco sobre caminhos relativos e absolutos. Tente entender como navegar pelas suas pastas usando caminhos relativos e quais as vantagens de usar um ou outro.

## 😎 AMBIENTE DE DESENVOLVIMENTO

Não perca muito tempo nisso. Instale o VSCode e ele vai dar conta da maior parte das coisas.

O VSCode é um editor de texto extensível. Você pode instalar extensões para que ele faça mais e mais coisas, mas por padrão ele já vai suportar várias linguagens de programação e facilitar a sua vida.

Dependendo do seu caso o VSCode pode não ser o ideal infelizmente, por isso eu vou deixar algumas recomendações aqui:

> Caso você tenha um computador mais lento:

- Sublime Text 4
- Notepad ++
- Kate

> Caso você tenha um computador mais poderoso e muita grana sobrando:

- PHP Storm

> Caso você simplesmente não goste da Microsoft:

- Atom
- VSCodium

> Não recomendo usar estes no começo, mas caso você caia neles sem querer aqui vai a forma de sair:

- Vim _(Use Esc + :q! para sair)_
- NeoVim _(Use Esc + :q! para sair)_

## 👁️‍🗨️ Um pouco de código do lado do cliente

Um cliente pode ser qualquer outra máquina. Normalmente é um outro servidor que precisa que o seu servidor faça algo, um navegador web como o Chrome ou Firefox, um aplicativo de celular ou até mesmo um sistema embarcado em uma plantação no meio do Ceará.

O mais comum no nosso dia a dia é que nosso cliente seja um navegador. Nos navegadores vamos usar coisas como Javascript e formulários HTML para fazer requisições para o nosso servidor.

Recomendo que você estude um pouco sobre formulários HTML e sobre como fazer requisições com a função `fetch` no Javascript.

Caso você queira se aprofundar mais em frontend pode dar uma olhada nesse outro [link focado em HTML/CSS/JS](/FRONTEND.md)

## 🖥️ Um pouco de terminal

Essa é uma recomendação para facilitar a sua vida no dia a dia, mas você não precisa focar muito nisso.

Não há necessidade de virar um mestre do terminal agora, pode ver isso melhor depois.

Não é nada demais, mas tente se acostumar com o terminal e comece a usar comandos como `ls`, `cd`, `mdkir`, `touch`, `rm`, `grep`. Esses comando vão te ajudar a navegar pelo sistema de arquivos e a procurar por coisas quando você estiver programando.

## 🐘 PHP

PHP é uma linguagem de programação focada em construir aplicações web (backend).

É um pouco peculiar, mas é legal, simples, produtiva e quentinha. Temos muitas vagas para PHP no mercado também.

### 🤖 POR ONDE COMEÇAR

Vamos começar instalando o PHP. Você pode fazer isso por aqui:

**Se você usa Windows**:

- [Baixe o PHP por aqui](https://windows.php.net/download/)

> Se você está na dúvida entre quais das versões baixar vá na que tem "x64 Non Thread Sage" no título. Clique em "Zip" para baixar o PHP.

- Extraia os arquivos do arquivo `.zip` que você baixou.

- Copie os arquivos extraídos, crie uma pasta `C:\php` e cole eles lá dentro.

- Renomeie `C:\php\php.ini-development` para `C:\php\php.ini`. Este é um arquivo de configuração do PHP.

- Adicione o caminho `C:\php` em suas variáveis de ambiente do Windows. Procure por `ambiente` na barra de pesquisa, selecione _Editar variáveis de ambiente_, selecione _Avançado_ e então clique em _Variáveis de ambiente_. Procure por `path` abaixo de `Variáveis do Sistema` e adicione `C:\php`.

**Se você usa Linux:**

- Abra seu terminal e depois:

> Caso seu Linux seja um Debian, Ubuntu ou derivado use:

```bash
sudo apt-get update
sudo apt-get upgrade
sudo apt-get install php
```

> Caso seu Linux seja um Arch, Manjaro ou derivado use:

```bash
sudo pacman -Syu
sudo pacman -S php
```

---

Em uma pasta de sua escolha cria um arquivo `index.php` e dentro dele digite:

```php
<?php
echo "Olá mundo!";
```

Podemos executar código PHP pelo terminal com:

```bash
php index.php
```

Ou podemos executar o código PHP e ver sua saída em uma página web com:

```bash
php -S localhost:3030
```

É importante lembrar que você deve estar executando o comando no mesmo diretório que o arquivo `index.php`.

---

Vamos agora pontuar alguns tópicos de estudo:

- Como funciona a execução de um código PHP ?

- Variáveis e seus tipos

- Operadores matemáticos

- Funções úteis para lidar com números e matemática

- Strings

- Funções úteis para lidar com strings

- Operadores lógicos

- Estruturas condicionais

- Arrays e funções úteis para lidar com arrays

- Valores truthy e falsy

- Estruturas de repetição

- Arrays associativos

- Iterar sobre arrays com foreach

- Obter input do usuário

- Funções

- Escopo de variáveis em funções

- Conceito de refatoração

- Acessar o sistema de arquivos

- Como separar seu código em funções e arquivos diferentes

- Refatoração de execícios anteriores para usar funções _(Caso tenha feito, se não fez... deveria ter feito)_

- Introdução a Regex _(Expressões regulares)_

- Validando strings com Regex

- Introdução a Orientação a Objetos

- Conceito de abstração e como isso pode ser representado em um código PHP

- Exemplos de abstrações

- Conceito de encapsulamento, como isso está presente em um código PHP e porque é importante

- O que são Getters e Setters?

- Conceito de herança, como isso está presente em um código PHP e porque é importante

- Criar classes que utilizem herança para explorar problemas e possibilidades

- Conceito de polimorfismo e como explicar isso para uma criança de 8 anos, para um adulto de 18 e para um profissional de 40

- Representar elementos em uma classe

- Herança vs Composição

- O que é CRUD?

- Criar uma aplicação CRUD simples com PHP (Sem banco de dados)

- Refatorar essa aplicação para ter mais _Abstração_ e _Encapsulamento_

- O que é MVC?

- Refatorar a aplicação anterior para seguir o modelo MVC (Ainda sem banco de dados)

- Introdução ao SQL

- Como se conectar a um banco de dados no PHP

- O que é o PDO?

- Como utilizar o PDO para se conectar a um banco de dados

- Como gravar dados no banco de dados com PHP

- Como evitar que o usuário envie dados incorretos ou maliciosos para guardarmos no banco de dados

- Como limpar os dados que o usuário enviou

- Conceito de hash e criptografia

- Por que e como fazer o hash de senhas do usuário antes de guardar no banco de dados?

- Sessões no PHP

- Fazer um cadastro e login de usuários na aplicação anterior (crud) ou em uma nova

## 🚨 IDEIAS DE PROJETOS

- Sorteador de frases aleatórias
- Lista de coisas para fazer (Todo list)
- Lista de coisas para fazer (Com login desta vez)
- Listar filmes
