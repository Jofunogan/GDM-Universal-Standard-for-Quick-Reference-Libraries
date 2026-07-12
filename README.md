# GDM-USQRL

## Gana.dm Universal Standard for Quick Reference Libraries

---

# Sobre

GDM-USQRL é uma especificação de organização de dados baseada em arquivos JSON para criação de bibliotecas de consulta rápida.

A especificação define uma estrutura padronizada para organizar informações de forma simples, consistente e acessível.

Não é um aplicativo, programa, linguagem ou plataforma. É uma convenção de estruturação de dados que define como arquivos JSON podem ser organizados para representar bibliotecas de referência rápida.

---

# Objetivo

A estrutura foi criada para facilitar o armazenamento, organização e consulta de informações.

O objetivo é permitir que diferentes tipos de conhecimento possam ser organizados seguindo um modelo comum.

A estrutura permite:

- Organização consistente de informações.
- Consulta rápida de conteúdos específicos.
- Separação entre organização e dados.
- Leitura por humanos e aplicações.
- Reutilização dos dados em diferentes projetos.

---

# Aplicações

A especificação não é limitada a uma área específica.

Pode ser utilizada para criar bibliotecas de qualquer tipo de conhecimento, incluindo:

- Documentação técnica.
- Estudos pessoais.
- Materiais educacionais.
- Ciências.
- História.
- Idiomas.
- Referências profissionais.
- Coleções de informações.
- Programação e tecnologia.
- Qualquer outro conjunto organizado de conhecimento.

A finalidade da biblioteca depende do objetivo de quem a cria.

---

# Conceito

Uma biblioteca de consulta rápida organiza informações para que conteúdos específicos possam ser encontrados de forma eficiente.

A estrutura utiliza uma separação entre:

- Índices, responsáveis pela organização e navegação.
- Armazenamento, responsável pelos conteúdos individuais.

Essa separação permite que grandes coleções de informações sejam organizadas sem depender de um único arquivo contendo todos os dados.

---

# Estrutura Geral

Uma biblioteca segue uma organização hierárquica:

```
Biblioteca

├── Índices

└── Conteúdos
```

A relação entre os dados segue:

```
Biblioteca

↓

Grupos

↓

Itens individuais
```

---

# Arquitetura de Arquivos

Exemplo de organização:

```
biblioteca/

├── index.json

├── groups/

│   ├── grupo-1.json

│   ├── grupo-2.json

│   └── grupo-3.json

└── storage/

    └── nome-da-biblioteca/

        ├── nome-do-grupo/

        │   ├── item-001.json

        │   ├── item-002.json

        │   └── item-003.json
```

---

# Index

O arquivo principal `index.json` contém informações gerais da biblioteca.

Ele pode definir:

- Identificação da biblioteca.
- Informações gerais.
- Localização dos grupos.
- Relações principais da estrutura.

---

# Grupos

Os grupos representam divisões internas utilizadas para organizar conteúdos relacionados.

Eles funcionam como índices intermediários entre a biblioteca e os itens individuais.

Exemplo:

```
Biblioteca

├── Grupo A

├── Grupo B

└── Grupo C
```

Cada grupo possui informações que permitem localizar e organizar seus respectivos itens.

---

# Storage

A pasta `storage` contém os arquivos individuais com os conteúdos completos.

A organização segue:

```
storage/

└── biblioteca/

    └── grupo/

        └── item.json
```

Cada arquivo representa uma unidade independente de informação.

---

# Itens

Os itens representam a menor unidade de informação dentro da estrutura.

Um item pode representar qualquer tipo de conteúdo:

- Conceito.
- Referência.
- Definição.
- Elemento.
- Comando.
- Informação específica.
- Registro de conhecimento.

Exemplo:

```json
{
  "id": "example-item",
  "title": "Título do item",
  "subtitle": "Informação complementar",
  "description": "Descrição do conteúdo."
}
```

---

# Separação entre Estrutura e Conteúdo

A organização diferencia duas partes principais.

## Estrutura

Responsável por:

- Índices.
- Grupos.
- Referências.
- Caminhos dos arquivos.
- Organização da biblioteca.

## Conteúdo

Responsável por:

- Títulos.
- Descrições.
- Exemplos.
- Informações específicas dos itens.

Essa separação permite que diferentes aplicações utilizem os mesmos dados.

---

# Dados Técnicos e Conteúdo Natural

Os arquivos possuem informações destinadas a diferentes objetivos.

## Dados Técnicos

Utilizados para identificação, referência e organização.

Exemplo:

```json
{
  "id": "example-item"
}
```

## Conteúdo Natural

Utilizado para apresentar informações compreensíveis para pessoas.

Exemplo:

```json
{
  "title": "Título do item",
  "description": "Descrição do conteúdo."
}
```

Os campos técnicos seguem uma estrutura definida pela especificação.

Os conteúdos textuais podem ser escritos no idioma escolhido pelo criador da biblioteca.

---

# Idioma

A especificação não define um idioma obrigatório.

Cada biblioteca pode utilizar o idioma mais adequado ao seu objetivo, público ou contexto.

Uma biblioteca pode ser:

- Pessoal.
- Interna de um projeto.
- Pública.
- Destinada a uma comunidade específica.
- Multilíngue, quando necessário.

A criação de traduções é opcional.

A universalidade está na estrutura dos dados, não no idioma utilizado.

---

# Compatibilidade

Qualquer aplicação capaz de interpretar arquivos JSON seguindo a estrutura definida pode utilizar uma biblioteca compatível.

A especificação permite diferentes implementações sem depender de uma aplicação específica.

---

# Licença

GDM-USQRL é uma especificação aberta para organização de bibliotecas de consulta rápida utilizando arquivos JSON.