# Proposta de Presença Digital — Vó Lila Gastrobar

Página única de apresentação (`index.html`) em HTML + CSS + JS puro, responsiva (mobile-first) e sem dependências externas além do Google Fonts.

## Estrutura de arquivos

```text
vo-lila/
├── index.html
├── README.md
└── assets/
    ├── logo-vo-lila.webp
    └── prints/
        ├── 01.webp
        ├── 02.webp
        └── 03.webp
```

## O que foi alterado nesta atualização

- **Prints reais em `.webp` e grid de 3 cards:** atualizados para `assets/prints/01.webp` (Anota), `assets/prints/02.webp` (Perfil no Google) e `assets/prints/03.webp` (Tripadvisor), com `object-fit: contain` (sem cortar partes úteis da imagem), remoção do texto `"Print em breve"` e remoção completa do card do Linktree (PRINT 04), ajustando o layout para 3 cards alinhados (3 colunas no desktop e 1 coluna no celular).

- **Nova seção ("Nome, endereço e telefone: onde o cliente se confunde"):** inserida entre o Diagnóstico em 4 pontos e a Proposta em duas etapas (`#canais`), com tabela responsiva que se transforma em cartões empilhados no celular (375px, sem rolagem horizontal, texto mínimo de 16px) e linha de cabeçalho em bronze no desktop, seguida da caixa de destaque explicando a padronização com aprovação do dono.
- **Etapa 1 (Perfil no Google):** adicionados os 3 itens de consistência cadastral (*"Padronizar nome, endereço e telefone com a placa da fachada"*, *"Conferir o ponto no mapa e o CEP"* e *"Corrigir o telefone principal, se necessário"*), mantendo todos os itens anteriores.
- **Etapa 2 (Página oficial mobile-first):** adicionado o item *"Nome, endereço e telefone idênticos aos do Google, no rodapé e nos dados estruturados da página"*.
- **Próximos passos (Passo 2 — "Ajuste de Google e diretórios"):** texto atualizado para *"Padronização de nome, endereço e telefone no Google e nos diretórios, e reivindicação da página no Tripadvisor."*
- **Destaque visual dos marcadores `[A CONFIRMAR]` e `[PREÇO]`:** estilizados com cor de atenção (`.tag-placeholder` com fundo e borda de alerta e contraste AA) para facilitar a revisão visual do que falta preencher.
- **Revisões anteriores mantidas:** nome `"Vó Lila Gastrobar"` padronizado com `white-space: nowrap`, `--madeira: #5C4234`, borda única por cartão, botões com mínimo de `44px` de altura e textos com mínimo de `16px` no celular.

---

## Lista de dados marcados como `[A CONFIRMAR]` que precisam ser checados

1. **Tabela comparativa de canais (`#canais`):**
   - **Instagram e logo:** Telefone exibido na bio/perfil `[A CONFIRMAR]`.
   - **Anota (delivery):** Endereço cadastrado `[A CONFIRMAR]` e Telefone cadastrado `[A CONFIRMAR]`.
   - **Link da bio (Linktree):** Endereço `[A CONFIRMAR]` e verificação do botão de WhatsApp com número de 8 dígitos `[A CONFIRMAR]`.
   - **Tripadvisor:** Endereço exibido na página `[A CONFIRMAR]` e Telefone exibido `[A CONFIRMAR]`.
2. **Canais de WhatsApp (Diagnóstico Cartão 04, Etapa 2, Mockup e Passo 1):**
   - Confirmar quais são os dois números de WhatsApp oficiais (delivery/encomendas e reservas) e se o telefone `(88) 99781-0603` do Google deve ser mantido como principal.
3. **Mockup da página oficial (`#mockup`):**
   - Frase curta de apresentação abaixo do título: `[A CONFIRMAR] frase de apresentação`.
4. **Proposta em duas etapas (`#proposta`) e Agendamento (`#proximos-passos`):**
   - Prazo estimado da Etapa 2 (`[A CONFIRMAR]`).
   - Valores de investimento da Etapa 1 e da Etapa 2 (`[PREÇO]`).
   - Link de agendamento no botão **"Agendar alinhamento de 10 minutos"** (`[LINK]`).

---

## Onde editar antes de enviar ao cliente

### 1. Trocar a paleta de cores
No arquivo `index.html`, localize o bloco `:root` (logo no início da tag `<style>`, linha 19) e altere os códigos hexadecimais caso o cliente envie a paleta oficial:

```css
:root {
  --preto: #141414;
  --creme: #F4EDE1;
  --madeira: #5C4234;
  --bronze: #B08A4E;
  --verde: #2E3A2A;
}
```

### 2. Prints do diagnóstico
Os 3 prints ativos ficam em `assets/prints/` (o antigo card 04 do Linktree foi removido):
- `assets/prints/01.webp` — Captura do Anota em 17/11/2026, 17h34: loja de delivery exibida como offline em horário de funcionamento.
- `assets/prints/02.webp` — Perfil no Google com o nome 'Vó Lila Gastro-bar' (com hífen), nota 4,4 com 294 avaliações e botão de pedido apontando para o Anota.
- `assets/prints/03.webp` — Página no Tripadvisor com o nome 'Vo Lila Cafe Gourmet', ainda não reivindicada pelo negócio.

### 3. Atualizar links, preços e dados a confirmar
No arquivo `index.html`, faça uma busca (`Ctrl + F`) por `[A CONFIRMAR]`, `[PREÇO]` e `[LINK]` para substituir pelos dados finais validados.

# proposta_vo_lilla-2
