# Guia de estudo — Módulo 01

Hugo Nunes · 881942 · Licenciatura em Informática · Revisão: 07/10/2026

## Estrutura de uma página

- `<!DOCTYPE html>` indica HTML5.
- `html lang="pt-PT"` identifica o idioma, útil para leitores de ecrã.
- `head` contém os metadados; `body` contém o conteúdo da página.
- `meta charset="UTF-8"` permite representar os acentos. `meta name="author"` identifica o autor.
- `meta name="viewport"` ajusta a área de visualização à largura do dispositivo; não torna, por si só, todos os conteúdos adaptáveis.
- `title` dá nome ao separador do navegador; `h1` apresenta o título principal. `h2` e `h3` organizam assuntos e subassuntos.
- `p` representa um parágrafo. `ul` cria uma lista sem ordem obrigatória; `ol` uma lista ordenada; `li` cada item. `br` introduz uma mudança de linha.

## Semântica — EX01 e EX02

| Elemento | Função |
| --- | --- |
| `header` | Introdução da página ou de um artigo. |
| `nav` | Conjunto de ligações de navegação. |
| `main` | Conteúdo principal da página. |
| `section` | Grupo temático, normalmente com um título. |
| `article` | Conteúdo independente, como uma notícia ou apresentação de um projeto. |
| `aside` | Informação complementar, como a nota de aprendizagem. |
| `footer` | Informação final e ligações de regresso. |

Os elementos são escolhidos pelo significado do conteúdo. No EX02, as competências estão em aprendizagem; os projetos são os exercícios do módulo.

## Ligações, âncoras e imagens

`a` cria uma ligação e `href` indica o destino. `../index.html` sobe uma pasta; `about.html` abre um ficheiro na mesma pasta. `mailto:` prepara uma mensagem na aplicação de email, sem a enviar automaticamente.

`href="#biografia"` procura `id="biografia"` na mesma página. `index.html#ia` abre outra página e procura a respetiva âncora. Cada ID deve ser único dentro da página.

`img src="imagens/perfil.jpg"` usa uma imagem local. `alt` descreve o conteúdo relevante; `width` e `height` indicam as dimensões de apresentação. `figure` agrupa a imagem e `figcaption` dá a legenda. A fotografia do perfil é temática, não um retrato.

## Notícias — EX03

O índice tem cinco `article`, cada um ligado a uma página completa. Cada notícia inclui título, autor, data, categoria e imagem. O `header` dentro de um artigo apresenta os dados dessa notícia.

`time datetime="2026-10-06"` associa o texto da data a um valor padronizado. As datas pertencem às notícias fictícias; são diferentes da data de revisão do trabalho.

## Formulários — EX04 e contactos do EX05

| Elemento ou atributo | O que faz |
| --- | --- |
| `form` | Agrupa os campos e os botões. |
| `action="recebido.html"` | Define o destino da submissão. |
| `method="get"` | Coloca os valores no endereço do destino. |
| `fieldset` e `legend` | Agrupam campos e dão nome ao grupo. |
| `label for="nome"` | Associa o texto ao campo com `id="nome"`. |
| `id` e `name` | ID identifica o elemento; name identifica o valor submetido. |
| `type="text"`, `email`, `tel` | Recebem texto, email e telefone. Email verifica um formato básico; tel não impõe um formato sozinho. |
| `autocomplete` | Indica o tipo de dado para ajudar o preenchimento automático. |
| `textarea`, `rows`, `cols` | Recebe texto em várias linhas; rows e cols definem o tamanho inicial. |
| `select`, `option`, `value` | Apresentam escolhas e definem o valor enviado. |
| `type="checkbox"` | Cria uma caixa de seleção. |
| `button type="submit"` | Tenta validar e submeter o formulário. |
| `button type="reset"` | Repõe os valores iniciais. |

`required` exige preenchimento. Uma opção com `value=""` não satisfaz um select obrigatório. `minlength` e `maxlength` limitam o comprimento dos textos. Não confirmam a veracidade dos dados.

O padrão `[+]?[0-9]{9,15}` aceita um sinal + opcional e entre 9 e 15 algarismos, sem espaços. Como o telefone não tem required, pode ficar vazio. A validação ocorre no navegador; um servidor real teria de voltar a validar os dados.

`aria-label` dá um nome acessível à navegação. `aria-describedby` associa um campo ou formulário à ajuda identificada por um ID. Não substituem os labels visíveis.

O destino local não processa nem envia mensagens. GET deixa os valores no endereço e pode deixá-los no histórico. Abrir recebido.html diretamente não prova que o formulário foi submetido.

## Navegação e FAQ — EX05

A mesma navegação liga as cinco páginas da empresa e aparece também no destino do formulário. `details` cria uma resposta que abre e fecha; `summary` é o título clicável. O atributo booleano `open` deixa a primeira resposta inicialmente aberta. Funciona sem JavaScript.

## Roteiro para a apresentação e testes manuais

1. Abrir o índice e explicar a organização das pastas e dos caminhos relativos.
2. No EX01, mostrar títulos, lista, imagem e ligação. No EX02, clicar nas quatro âncoras e no regresso ao topo.
3. No EX03, abrir as cinco notícias e mostrar os dados e imagens.
4. Em ambos os formulários, tentar submeter vazio. Depois testar email inválido, nome com um carácter, assunto com dois, mensagem com nove, telefone com letras ou espaços, seleção vazia e checkbox desmarcada.
5. Preencher com Pessoa Teste, teste@example.com, +351912345678, um tipo selecionado, Pedido de teste e Esta é uma mensagem de teste. Marcar a checkbox e submeter; confirmar recebido.html e os parâmetros no endereço. Repetir com telefone vazio.
6. Testar Limpar campos e a navegação com Tab, Shift+Tab, Enter e espaço nos controlos adequados.
7. Percorrer as páginas da empresa e abrir e fechar a FAQ.

Na revisão foram executados controlos estáticos das 17 páginas, 132 referências locais, IDs, âncoras, labels, ajudas, fechos dos elementos e ausência de CSS e JavaScript. Foram confirmadas as cinco notícias e a navegação consistente da empresa. Os oito ficheiros de imagem foram mantidos sem alteração durante a revisão dos textos.

Os testes de validação e submissão no navegador não foram executados: a ferramenta de navegador não estava disponível. Os controlos estáticos não substituem um validador completo de HTML5 ou os testes manuais acima.

## Correspondência com o enunciado

A comparação foi feita com as seis páginas do PDF do Módulo 01.

| Exercício | Nível | Requisitos presentes no código |
| --- | --- | --- |
| EX01 | L1 | DOCTYPE, html, head, body, title, títulos, parágrafos, imagem, ligações, lista, header, main e footer. |
| EX02 | L1 | header, nav, main, section, article, aside e footer, com navegação interna por âncoras e sem div. |
| EX03 | L2 | Cabeçalho, navegação e cinco notícias com autor, data, categoria, imagem e ligações. Bónus: cinco páginas individuais. |
| EX04 | L2 | Nome, email, telefone, assunto, mensagem, seleção, checkbox e submit, com labels e tipos apropriados. Bónus: atributos de validação HTML5. |
| EX05 | L3 | index.html, about.html, services.html e contact.html, com navegação consistente. Bónus: faq.html. |

A presença dos requisitos foi confirmada por leitura do código e controlos estáticos. A abertura das páginas, a interação com a FAQ e a validação e submissão dos formulários continuam a exigir os testes no navegador descritos acima.

A entrega é no repositório GitHub m01 até 09/10/2026 às 23h59m59s. O módulo vale nove pontos e exige pelo menos cinco para aprovação, após avaliação das soluções e explicação dos conceitos.
