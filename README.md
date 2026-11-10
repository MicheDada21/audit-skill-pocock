# audit-skill-pocock

Rivede una skill regola per regola con le indicazioni di Matt Pocock sulla scrittura per agenti e le aggiunte di Theo, poi propone un piano di riscrittura. Parte solo quando la chiami per nome.

Fa parte della [Prompt Library di CH Labs](https://www.cryptohelvetia.com/ch-labs/prompt-library), dove la pagina di riferimento è [Audit skill Pocock](https://www.cryptohelvetia.com/ch-labs/prompt-library/skills/audit-skill-pocock). Il repo contiene una copia della skill, rigenerata a ogni aggiornamento della libreria.

## Installare

In Claude Code aggiungi una volta il marketplace e installa il plugin.

```
/plugin marketplace add MicheDada21/ch-labs-skills
/plugin install audit-skill-pocock@ch-labs-skills
```

Da shell i comandi sono `claude plugin marketplace add MicheDada21/ch-labs-skills` e `claude plugin install audit-skill-pocock@ch-labs-skills`. Nell'app desktop premi + accanto al campo del prompt, apri Plugins, aggiungi il marketplace `MicheDada21/ch-labs-skills` con Add marketplace e poi il plugin con Add plugin.

Per avere tutte le skill della libreria installa `tutte-le-skill@ch-labs-skills`. Con altri agenti copia la cartella `skills/audit-skill-pocock` tra le skill dell'agente, per esempio in `~/.codex/skills/audit-skill-pocock`.

## Licenza

MIT, testo completo in [LICENSE](LICENSE).
