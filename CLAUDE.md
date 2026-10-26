# Elife — landing page Consumidores Sintéticos

## Como publicar alterações — OBRIGATÓRIO

Todas as alterações, em qualquer site da Elife/AIhub, seguem **sempre** este circuito:

**alteração → commit + push para o GitHub (`master`) → o Vercel faz o deploy automático → site atualizado**

- Depois de alterar ficheiros: `git add`, `git commit`, `git push origin master`. Não pedir confirmação para o push.
- **Nunca** publicar com `vercel --prod` / `npx vercel` nem editar diretamente no dashboard do Vercel — isso salta o GitHub e a versão seguinte apaga a alteração.
- Depois do push, confirmar que o deploy no Vercel ficou **Ready** e que o site responde.

### Contas

- **GitHub:** `aihub-cloud`
- **Vercel:** conta hub.ai@elifeportugal.com, equipa **"AI Hub"** (`ai-hub-5dd9`, `team_6cgk7fWRD8FtyslO5Llck3N7`). Domínios `elifeportugal.com` e `aihubdigital.com` também estão nesta equipa (DNS gerido fora do Vercel).
- A conta Vercel antiga (goncaloferreira, equipa `ai-hub1` / `team_XXgsVUKVe5JBs4sJ9JN25DXq`) foi **apagada em outubro de 2026**. Qualquer referência a ela, a `vercel --prod` ou a GitHub Actions de deploy está obsoleta.

### Mapa repositório → projeto Vercel → site

| Repositório GitHub (pasta) | Projeto Vercel | Site |
|---|---|---|
| `elife-website` | elife-portugal | www.elifeportugal.com |
| `aihub-site` | aihub-site | aihub.elifeportugal.com |
| `aihub-inscricao` (`Webinar/`) | aihub-webinar | webinar.aihub.elifeportugal.com |
| `aihub-inscricao` (`Inscrição/`) | aihub-inscricao | eventos.aihub.elifeportugal.com |
| `aihub-inscricao` (`AIhub Obrigado/`) | inscricao-obrigado | inscricao-obrigado.vercel.app |
| `elife-workshop-lisboa-out2026` | elife-workshop-lisboa-out2026 | redireciona para www.elifeportugal.com/eventooutubro26 |
| `lp-consumidores-sint` | lp-consumidores-sint | lp-consumidores-sint.vercel.app |

Os repositórios `aihub-webinar` e `aihub-eventos` são versões antigas, já não ligadas a nenhum site — não editar.
