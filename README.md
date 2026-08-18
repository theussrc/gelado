# Página de Vendas — Gel Gelado de Massagem

## ⚠️ Checklist ANTES de publicar (faça isso primeiro)

- [ ] **Trocar o link do botão de compra.** Abra `index.html`, procure por `href="#"`
      no botão final ("Quero o meu Gel Gelado →") e cole o link de checkout real
      da Kaiross (formato `https://pay.kairross.com.br/xxxxx`).
- [ ] **Trocar as imagens placeholder.** Procure por `product-placeholder` e
      `visual-block` no HTML — hoje são caixas com texto substituto. Troque por
      `<img src="...">` com as fotos reais do produto (as que você já tem).
- [ ] **Depoimentos.** A seção "O que as pessoas sentem" está com nomes fictícios
      `[nome do cliente]`. Só publique com depoimentos reais de clientes de
      verdade — depoimento inventado é propaganda enganosa e é ilegal, além do
      risco de banimento em plataformas de anúncio.
- [ ] Revisar o preço (`R$ 129,90`) — já está certo, só confirme antes de subir.

## Como publicar na Vercel

### Opção mais simples — Vercel CLI (sem precisar de GitHub)
1. Instale a CLI (se ainda não tiver): `npm i -g vercel`
2. Dentro desta pasta, rode: `vercel`
3. Siga as perguntas no terminal (login, nome do projeto, etc.) — aceite os
   padrões.
4. Ao final ele te dá uma URL tipo `https://sua-pagina.vercel.app`.
5. Pra apontar um domínio próprio depois: `vercel domains add seudominio.com`

### Opção via GitHub (recomendada se for atualizar com frequência)
1. Crie um repositório no GitHub e suba esta pasta (`index.html`,
   `vercel.json`).
2. Entre em [vercel.com](https://vercel.com) → **Add New Project** → conecte
   sua conta do GitHub → selecione o repositório.
3. Framework: deixe como **Other** (é HTML puro, sem build).
4. Clique em **Deploy**.
5. Toda vez que você der push no GitHub, a Vercel atualiza o site sozinha.

Nenhuma das duas opções precisa de build step — é HTML/CSS puro, então o
deploy é praticamente instantâneo.
