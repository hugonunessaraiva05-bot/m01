Trabalho realizado por: Hugo Nunes, número mecanográfico: 881942. Curso: Licenciatura em Informática. Data: 07/10/2026.

Instituição: Instituto Superior Miguel Torga (ISMT).

Unidade curricular: Programação Web.

# Módulo 01 — Programação Web

Cinco exercícios para praticar a estrutura, a semântica e as interações nativas de HTML5.

## Exercícios

| Exercício | Solução |
| --- | --- |
| [EX01 — Página pessoal (L1)](ex01/index.html) | Apresentação, curso, temas de aprendizagem, imagem local, lista e ligações de contacto e recursos. |
| [EX02 — Perfil semântico (L1)](ex02/index.html) | Biografia, competências em aprendizagem, projetos e contactos, com elementos semânticos e âncoras para as secções e o topo. |
| [EX03 — Jornal tecnológico (L2)](ex03/index.html) | Cinco notícias com título, autor, data, categoria e imagem, ligadas a cinco páginas individuais. |
| [EX04 — Formulário de contacto (L2)](ex04/index.html) | Nome, email, telefone opcional, tipo de contacto, assunto, mensagem e confirmação, com labels e validação HTML5. |
| [EX05 — Website empresarial (L3)](ex05/index.html) | Início, sobre nós, serviços, contactos e FAQ, com navegação consistente e respostas que abrem e fecham. |

## Decisões principais

- Apenas HTML5, sem CSS, JavaScript ou bibliotecas.
- Pastas ex01 a ex05 diretamente na raiz, com caminhos relativos e imagens locais preservadas.
- Textos em português de Portugal; competências descritas como aprendizagem, sem acrescentar experiência ou qualificações.
- Notícias e empresa identificadas como fictícias. As fotografias são ilustrativas; as suas fontes estão em [FONTES_IMAGENS.md](FONTES_IMAGENS.md).
- Os dois formulários usam GET para abrir recebido.html. Não processam pedidos nem enviam email; os valores ficam no endereço e podem permanecer no histórico. Usar dados fictícios.

## Como abrir

Abre [index.html](index.html) num navegador e escolhe um exercício. Não é necessária instalação nem servidor. Mantém as pastas e imagens nos seus locais. A documentação externa requer Internet; as ligações mailto dependem da aplicação de email configurada.

Consulta [GUIA_ESTUDO.md](GUIA_ESTUDO.md) para preparar a apresentação.

## Logótipo da instituição

O logótipo oficial do ISMT ainda não foi fornecido. Coloca o ficheiro em `imagens/ismt.png`, criando a pasta `imagens` na raiz do projeto. Se a imagem tiver outro formato, conserva a extensão correspondente.

Quando o ficheiro estiver disponível, adiciona ao cabeçalho do `index.html` principal uma imagem com caminho relativo `imagens/ismt.png` e `alt="Logótipo do Instituto Superior Miguel Torga"`. Define apenas a largura (por exemplo, `width="200"`) para manter as proporções originais, sem CSS ou JavaScript.

## Entrega

O enunciado define um repositório GitHub chamado `m01`, com cada exercício na sua pasta `ex01` a `ex05`, e o prazo de **09/10/2026 às 23h59m59s**. Publica esta raiz no repositório, incluindo o README, o guia e as imagens locais.

Os cinco exercícios totalizam nove pontos. A aprovação exige pelo menos cinco pontos, com soluções consideradas válidas e capacidade de explicar o código; a entrega também implica avaliação por um colega e, possivelmente, pelo professor.
