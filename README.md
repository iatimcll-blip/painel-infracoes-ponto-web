# Painel de Infrações de Ponto por GA

Front-end estático (HTML + JS, sem build) do painel de infrações de ponto. Este repositório é público, mas **não contém nenhum dado sensível** — é só a interface. Os dados reais (nomes, matrículas, infrações) ficam em um banco Supabase protegido por autenticação e Row Level Security, e só aparecem depois de login com uma conta autorizada.

## Stack

- HTML/CSS/JS puro, sem framework.
- [Chart.js](https://www.chartjs.org/) para os gráficos.
- [Supabase](https://supabase.com/) para autenticação (email/senha) e para servir os dados via REST API, com acesso restrito a usuários autenticados.

## Rodando localmente

Basta servir a pasta com qualquer servidor estático, por exemplo:

```bash
python -m http.server 8000
```

Acesse `http://localhost:8000` e faça login com uma conta cadastrada no projeto Supabase.

## Publicado em

GitHub Pages, a partir da branch `main`.
