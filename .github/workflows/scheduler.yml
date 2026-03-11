name: Monitoramento a cada 30 min

on:
  schedule:
    # O comando abaixo diz: "No minuto zero e no minuto 30 de cada hora"
    - cron: '*/30 * * * *'
  
  # Recomendado para testar manualmente sem esperar 30 min
  workflow_dispatch:

jobs:
  ping-servidor:
    runs-on: ubuntu-latest
    steps:
      - name: Verificar se o site esta online
        run: |
          curl -I https://glorious-charleen-lealcyber-36e30d5e.koyeb.app/from_github
          echo "Verificacao concluida em: $(date)"