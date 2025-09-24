# Mapa Interativo do Porto — Freguesias + Pins

Este repositório contém um **mapa interativo** da cidade do Porto, com **delimitação de freguesias** e suporte para **pins** (empreendimentos, pontos de interesse), importação/exportação **GeoJSON/CSV**, zoom e pan sem perda de qualidade.

- Base tecnológica: [Leaflet](https://leafletjs.com/) + [OpenStreetMap](https://www.openstreetmap.org/)
- Limites das freguesias: serviço ArcGIS disponibilizado pela **Águas do Porto** (GeoJSON).
- Licença: MIT (código). Dados de terceiros regem-se pelas respetivas licenças.

---

## Como publicar **gratuitamente** com GitHub Pages

1. Crie um repositório público (ex.: `mapa-porto`).
2. Carregue os ficheiros deste projeto (pelo menos `index.html` e `pins-template.csv`).
3. No repositório, aceda a **Settings → Pages** e selecione:
   - **Source**: *Deploy from a branch*
   - **Branch**: `main` (ou `master`), pasta `/root`
4. Guarde. O GitHub criará um URL do tipo:
   `https://<o-seu-utilizador>.github.io/mapa-porto/`
   - A página principal será `index.html`.
5. Abra o link e teste.

> **Dica:** Se quiser usar domínio próprio, adicione um ficheiro `CNAME` com o domínio e aponte o DNS conforme a documentação do GitHub Pages.

---

## Utilização

- **Adicionar pin**: clique em “Ativar modo Adicionar Pin”, indique *Nome* e *Notas*, e clique no mapa.
- **Mover pin**: arraste o pin para a posição correta.
- **Importar**:
  - **CSV** com colunas `name,notes,lat,lng` (ver `pins-template.csv`).
  - **GeoJSON** de pontos.
- **Exportar**: clique em **Exportar pins (GeoJSON)**.
- **Rótulos**: pode ligar/desligar rótulos das freguesias.
- **Zoom/Pan**: use a roda do rato e arraste o mapa.

### Formato CSV (exemplo)
```csv
name,notes,lat,lng
Gramoínhos Living,Em construção; T2/T3,41.112345,-8.600123
Exemplo 2,Licenciado; T1/T2,41.160001,-8.620001
```

> **Nota:** Para obter coordenadas, pode usar o clique no mapa (após ativar o modo Adicionar Pin) e ler as coordenadas no popup, ou utilizar ferramentas externas (ex.: Google Maps → botão direito → “O que há aqui?”).

---

## Créditos e licenças

- **Map tiles e dados base**: © Contribuidores do OpenStreetMap (ODbL).
- **Leaflet**: Copyright © Vladimir Agafonkin e contribuidores (BSD 2-Clause).
- **Limites de freguesias**: serviço ArcGIS público da **Águas do Porto**.
- **Código deste repositório**: Licença MIT (ver `LICENSE`).

Este projeto é fornecido “tal como está”. Verifique sempre a atualidade dos limites administrativos (CAOP/DGT) para usos jurídicos/fiscais.
