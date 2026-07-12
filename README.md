# GDM-USQRL

## Gana.dm Universal Standard for Quick Reference Libraries

---

# Sobre

Especificação de organização de dados baseada em JSON para criação de bibliotecas de consulta rápida.

Define uma estrutura padronizada para organizar informações de forma simples, consistente e acessível.

Não representa um aplicativo, linguagem ou plataforma. É uma convenção de estruturação de dados que define como informações podem ser organizadas em arquivos JSON para representar bibliotecas de referência rápida.

---

# Objetivo

A estrutura foi criada para facilitar o armazenamento, organização e consulta de informações.

O objetivo é permitir:

- Organização consistente dos dados.
- Consulta rápida de informações específicas.
- Separação entre estrutura e conteúdo.
- Leitura por humanos e aplicações.
- Reutilização dos dados em diferentes projetos.

---

# Características

## Estrutura Padronizada

As bibliotecas seguem um modelo organizado de arquivos, grupos e itens.

A padronização permite que diferentes aplicações interpretem os mesmos dados utilizando uma estrutura comum.

---

## Baseado em JSON

Os dados são armazenados utilizando arquivos JSON.

O formato permite:

- Leitura humana.
- Processamento por aplicações.
- Fácil edição.
- Portabilidade entre projetos.

---

## Independência de Aplicação

A estrutura não depende de um software específico.

Qualquer aplicação capaz de interpretar os arquivos seguindo a estrutura definida pode utilizar as bibliotecas.

---

## Separação entre Estrutura e Conteúdo

A organização diferencia dados técnicos e informações destinadas à compreensão humana.

Dados técnicos:

```json
{
  "id": "query-selector"
}
```

Utilizados para identificação e organização.

Conteúdo natural:

```json
{
  "title": "Selecionar elemento",
  "description": "Retorna o primeiro elemento correspondente a um seletor CSS."
}
```

Utilizado para apresentar informações ao usuário.

---

# Idioma

A especificação não define um idioma obrigatório para o conteúdo das bibliotecas.

Cada criador pode utilizar o idioma mais adequado ao objetivo da biblioteca.

Uma biblioteca pode ser:

- Pessoal.
- Interna de um projeto.
- Destinada a uma comunidade específica.
- Pública.
- Multilíngue, caso seja necessário.

A tradução do conteúdo é opcional e depende da finalidade de cada projeto.

A estrutura dos dados permanece a mesma independentemente do idioma utilizado.

---

# Estrutura

Uma biblioteca segue uma organização hierárquica:

```
Biblioteca
│
├── Grupos
│
└── Itens
```

---

# Biblioteca

Representa uma coleção de informações relacionadas a um determinado assunto.

Exemplos:

```
HTML
JavaScript
CSS
Python
Matemática
```

---

# Grupos

Representam divisões internas utilizadas para organizar informações relacionadas.

Exemplo:

```
HTML

├── Elementos
├── Atributos
├── Eventos
└── Entidades
```

Os grupos facilitam a navegação e localização dos itens.

---

# Itens

Representam a menor unidade de informação dentro da estrutura.

Cada item contém uma referência específica, conceito, elemento, comando ou informação individual.

Exemplo:

```json
{
  "id": "query-selector",
  "title": "Selecionar elemento",
  "subtitle": "document.querySelector()",
  "description": "Retorna o primeiro elemento correspondente a um seletor CSS."
}
```

---

# Organização dos Dados

A estrutura separa:

## Estrutura

Responsável pela organização dos arquivos, grupos e itens.

## Conteúdo

Responsável pelas informações armazenadas dentro dos itens.

Essa separação permite que diferentes aplicações utilizem os mesmos dados.

---

# Licença

GDM-USQRL é uma especificação aberta para organização de bibliotecas de consulta rápida utilizando arquivos JSON.