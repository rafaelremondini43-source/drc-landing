# DRC — Landing Page

Landing page institucional da **DRC** — perfuração direcional pelo Método Não Destrutivo (MND / HDD).
Estática, single-page, sem framework. Mobile-first, acessível, motion contido.

## Stack
- `index.html` — página única (semântica + JSON-LD Organization/LocalBusiness).
- `css/styles.css` — design system navy (Roboto Condensed + Inter + Roboto Mono), cantos retos.
- `js/main.js` — Lenis (smooth scroll), reveals/contadores, nav, parallax, **drill-path** animado por scroll, menu mobile, envio do formulário por e-mail (mailto), mapa lazy.
- `js/lenis.min.js` — smooth scroll.
- `assets/img/` — fotos reais da DRC (otimizadas) + imagens geradas (Nano Banana Pro) + logo oficial.
- `assets/video/hero-loop.mp4` — loop do hero (Veo, a partir de foto real).
- `assets/src/` — originais (não servidos em produção).

## Regras do projeto
- **Logo:** somente o logo oficial da DRC (`assets/img/logo-drc.png`). Nunca substituir por outra marca.
- **Conteúdo:** a DRC **não** faz remediação de solo — o termo não deve aparecer.
- **Segmentos:** Energia, Gás/Óleo, Saneamento, Telecom, Infraestrutura Urbana (exatamente 5).

## Rodar localmente
Servir a pasta como estático, por exemplo:
```
npx serve .      # ou qualquer servidor estático
```

## Pendente (Fase B — não implementado)
Sistema de leads: projeto Supabase separado + tabela `leads` + envio por e-mail (Web3Forms/Formspree) + área interna com login para ler os formulários. O formulário já emite o evento `drc:lead` (em `js/main.js`) como gancho para essa integração. Hoje, sem backend, o envio abre o e-mail do visitante (mailto) com o resumo preenchido.
