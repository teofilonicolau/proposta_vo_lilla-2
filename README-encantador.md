# Vó Lila Gastrobar — Proposta de Presença Digital (6 Atos)

Apresentação interativa em arquivo único (`index.html`, gerada a partir de `index-encantador.html`), projetada para funcionar no celular, no computador e como documento PDF exportável em formato A4.

---

## 1. Como trocar a paleta de cores e os prints

### Paleta de cores (`:root`)
Abra o arquivo `index.html` e localize o bloco `:root` no início da tag `<style>` (por volta da linha 18):

```css
:root {
  --preto: #141414;
  --creme: #F4EDE1;
  --madeira: #5C4234;
  --bronze: #B08A4E;
  --verde: #2E3A2A;
}
```

### Prints da jornada (`assets/prints/`)
Substitua os arquivos mantendo os mesmos nomes na pasta `assets/prints/` (caso algum arquivo ainda não exista, o cartão exibirá automaticamente apenas a legenda `"Print em breve"`):
- `assets/prints/01.png` — Loja no Anota exibida como `"Loja offline"` às 17h34 (17/11/2026).
- `assets/prints/02.png` — Perfil da Empresa no Google (nota 4,4 com 294 avaliações e grafia `"Vó Lila Gastro-bar"`).
- `assets/prints/03.png` — Página no Tripadvisor com o nome antigo.
- `assets/prints/04.png` — Linktree na bio do Instagram com cardápio e os dois números de WhatsApp.

---

## 2. Onde ficam os marcadores `[A CONFIRMAR]`, `[PREÇO]` e `[LINK]`

Use `Ctrl + F` no arquivo `index.html` para localizar e preencher antes de enviar ao cliente:

- **`[A CONFIRMAR]`**:
  - **Ato 2 (Passo 2 — Abrir o Instagram):** confirmação dos dois números de WhatsApp presentes no Linktree.
  - **Ato 3 (Tabela NAP — O que encontramos):**
    - Telefone do canal *Instagram e logo*.
    - Endereço e Telefone do canal *Anota (delivery)*.
    - Endereço e número de WhatsApp de 8 dígitos do canal *Link da bio (Linktree)*.
    - Endereço e Telefone do canal *Tripadvisor*.
  - **Ato 4 (O que vamos fazer):** confirmação dos números de WhatsApp no comparador e na Etapa 2.
  - **Ato 5 (O investimento):** prazo de entrega da Implantação.
  - **Ato 6 (Próximo passo — Passo 1):** confirmação dos dois números de WhatsApp.
- **`[PREÇO]`**:
  - **Ato 5 (Tabela de Investimento):** valor da **Implantação (Etapas 1 e 2)** e valor da **Mensalidade**.
- **`[LINK]`**:
  - **Ato 6 (Próximo passo):** atributo `href="[LINK]"` no botão **"Agendar conversa de 10 minutos"**.

---

## 3. Como gerar o PDF (A4 pronto para envio)

1. Abra a página no navegador (Google Chrome ou Microsoft Edge) e clique no botão flutuante **"Baixar em PDF"** no canto inferior direito (ou pressione **`Ctrl + P`**).
2. No campo **Destino**, selecione **Salvar como PDF**.
3. Em **Tamanho do papel**, selecione **A4**.
4. Em **Mais definições**, marque a opção **Gráficos de segundo plano** (ou *Gráficos de fundo*) para preservar os quadros, cabeçalhos em bronze e destaques visuais.
5. Clique em **Salvar**. O modo de impressão (`@media print`) já remove automaticamente botões e controles interativos, expande as Etapas 1 e 2, posiciona o comparador *Antes e Depois* lado a lado em fundo claro e inclui a URL da página no rodapé.
