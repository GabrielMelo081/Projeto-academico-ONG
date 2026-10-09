# Casa Quatro Patas

Site institucional responsivo de uma ONG fictícia de resgate e adoção de cães e gatos. Projeto da 1ª Unidade (HTML5 e CSS3).

## 1. Apresentação do negócio

- **Nome do projeto:** Casa Quatro Patas
- **Segmento:** Social (ONG de proteção animal)
- **Público-alvo:** pessoas que querem adotar um animal, doadores e voluntários
- **Problema que o site resolve:** a ONG não tem presença digital, e quem quer adotar ou ajudar não sabe como fazer
- **Objetivo principal:** apresentar os projetos, explicar como adotar e facilitar doações e contato
- **Principais usuários:** futuros adotantes, doadores e voluntários
- **Diferencial:** adoção responsável, com entrevista, visita e termo, e animais entregues vacinados e castrados

## 2. Regras de negócio

| Código | Regra |
|---|---|
| RN01 | O site apresenta o serviço principal (resgate e adoção) na primeira dobra. |
| RN02 | Os canais de contato ficam a no máximo dois cliques (menu "Contato" e botões da primeira dobra). |
| RN03 | O formulário pede só nome, e-mail, assunto e mensagem. |
| RN04 | O site funciona em celular, tablet e desktop. |
| RN05 | Informações institucionais (Sobre, Projetos) ficam separadas das de ação (Doe, Contato). |
| RN06 | Toda imagem relevante tem texto alternativo. Ícones decorativos usam `alt=""`. |
| RN07 | O menu leva a todas as seções. |
| RN08 | O rodapé tem contato e links principais. |
| RN09 | A página explica o passo a passo da adoção antes do formulário. |
| RN10 | O botão "Quero adotar" leva direto ao formulário. |

## 3. Requisitos funcionais

- RF01: página inicial com apresentação (`#inicio`)
- RF02: menu de navegação (`<nav>` no topo)
- RF03: seção de projetos (`#projetos`)
- RF04: seção Sobre (`#sobre`)
- RF05: formulário de contato (`#contato`)
- RF06: rodapé com informações institucionais
- RF07: perguntas frequentes (`#perguntas`) e formas de ajudar (`#doe`)
- RF08: ilustrações e ícones em SVG coerentes com o tema

## 4. Requisitos não funcionais

- RNF01: responsivo, com `meta viewport` e media queries em `responsive.css`
- RNF02: HTML semântico (`header`, `nav`, `main`, `section`, `article`, `footer`)
- RNF03: CSS em arquivos externos
- RNF04: projeto organizado em pastas
- RNF05: texto escuro sobre fundo claro (e branco sobre azul-petróleo) com contraste adequado
- RNF06: imagens em SVG, leves
- RNF07: código indentado com 2 espaços
- RNF08: usa só recursos suportados pelos navegadores modernos

## 5. Arquitetura do projeto

```
casa-quatro-patas/
├── index.html          página única com todas as seções
├── css/
│   ├── reset.css       zera margens e define regras básicas
│   ├── style.css       cores, tipografia, layout (Flexbox) e componentes
│   └── responsive.css  ajustes para tablet e celular
├── assets/
│   └── img/            logo, ilustração e ícones (SVG)
└── README.md           esta documentação
```

## 6. Mapa do site

```
index.html
├── Início (#inicio)
├── Projetos (#projetos)
├── Sobre (#sobre)
├── Doe (#doe)
├── Perguntas frequentes (#perguntas)
└── Contato (#contato)
```

Foi escolhido o formato de uma página com 6 seções, e o menu rola até cada uma.

## 7. Wireframe (resumo)

```
+------------------------------------------+
| logo          Início Projetos Sobre ...  |  cabeçalho + menu
+------------------------------------------+
| Título grande          [ilustração]      |  seção principal
| [Quero adotar] [Quero doar]              |
+------------------------------------------+
| [card] [card] [card]                     |  cards
+------------------------------------------+
| Sobre | Como adotar (passos)             |
+------------------------------------------+
| Formulário            | Outros canais    |
+------------------------------------------+
| contato | links                          |  rodapé
+------------------------------------------+
```

Desenhe também um wireframe visual (Figma, Canva ou papel) para entregar.

## 8. Decisões visuais

- Paleta: azul-petróleo (confiança) e amarelo (acolhimento), sobre fundos claros
- Fontes: Fredoka nos títulos (arredondada, amigável) e Nunito Sans no texto
- A faixa azul da primeira dobra é o único bloco de cor forte, e o resto é limpo para dar atenção ao conteúdo
- O menu aumenta levemente (`transform: scale`) ao passar o mouse

## 9. Como rodar

Abra o `index.html` no navegador. Não precisa instalar nada.

## 10. Deploy (opcional)

1. Crie um repositório no GitHub e envie os arquivos.
2. Em Settings > Pages, escolha a branch `main` e a pasta raiz.
3. O site fica disponível em `https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO`.

## 11. O que melhorar numa próxima versão

- Trocar as ilustrações por fotos reais dos animais (em WebP, abaixo de 200 KB)
- Página de cada animal disponível para adoção
- Enviar o formulário de verdade (por exemplo, com um serviço de formulários)
- Menu recolhível no celular

## Pontos a personalizar

Troque os dados fictícios: e-mail, telefone, chave Pix, endereço e horário de atendimento.
