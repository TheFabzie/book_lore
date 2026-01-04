# Haus Connen

Familie aus Arden

## Stammbaum

```mermaid

%%{init: {"flowchart": {"curve": "linear", "nodeSpacing": 55, "rankSpacing": 80}} }%%
flowchart TB

%% ---------- Generation I (eine Zeile) ----------
subgraph Gen1[""]
direction LR
  harold_connen["✝ Harold Connen<br/>(535–601)"]
  maria_connen["✝ Maria Connen<br/>(541–598)"]
end
style Gen1 fill:transparent,stroke:transparent

e1((⚭))
harold_connen --- e1
maria_connen  --- e1

%% ---------- Generation II (eine Zeile, Reihenfolge erzwingen) ----------
subgraph Gen2[""]
direction LR
  %% Paar zuerst, dann Geschwister
  richard_connen["⭐ Richard Connen<br/>(567–)"]
  cathrine_markant["Cathrine Markant<br/>(571–)"]
  elizah_connen["Elizah Connen<br/>(569–)"]
  caroline_connen["Caroline Connen<br/>(574–)"]
end
style Gen2 fill:transparent,stroke:transparent

e1 --> richard_connen
e1 --> elizah_connen
e1 --> caroline_connen

%% ---------- Ehe Richard + Cathrine (zwischen den beiden) ----------
e2((⚭))
richard_connen --- e2
cathrine_markant --- e2

%% ---------- Generation III ----------
pascal_connen["Pascal Connen<br/>(596–)"]
e2 --> pascal_connen

%% ---------- Klickbare Links ----------
click harold_connen "/charaktere/harold-connen"
click maria_connen "/charaktere/maria-connen"
click richard_connen "/charaktere/richard-connen"
click elizah_connen "/charaktere/elizah-connen"
click caroline_connen "/charaktere/caroline-connen"
click cathrine_markant "/charaktere/cathrine-markant"
click pascal_connen "/charaktere/pascal-connen"


```
