# Haus Connen

Familie aus Arden

## Stammbaum

```mermaid

flowchart TB

%% ===== Generation I (eine Zeile) =====
subgraph Gen1["Generation I"]
direction LR
  harold_connen["✝ Harold Connen<br/>(535–601)"]
  e1((⚭))
  maria_connen["✝ Maria Connen<br/>(541–598)"]

  harold_connen --- e1
  e1 --- maria_connen
end

%% Kinder aus Ehe 1
e1 --> richard_connen["⭐ Richard Connen<br/>(567–)"]
e1 --> elizah_connen["Elizah Connen<br/>(569–)"]
e1 --> caroline_connen["Caroline Connen<br/>(574–)"]

%% ===== Generation II (eine Zeile) =====
subgraph Gen2["Generation II"]
direction LR
  richard_connen
  e2((⚭))
  cathrine_markant["Cathrine Markant<br/>(571–)"]
  elizah_connen
  caroline_connen

  richard_connen --- e2
  e2 --- cathrine_markant
end

%% Kind aus Ehe 2
e2 --> pascal_connen["Pascal Connen<br/>(596–)"]

%% Klickbare Links
click harold_connen "/charaktere/harold-connen"
click maria_connen "/charaktere/maria-connen"
click richard_connen "/charaktere/richard-connen"
click elizah_connen "/charaktere/elizah-connen"
click caroline_connen "/charaktere/caroline-connen"
click cathrine_markant "/charaktere/cathrine-markant"
click pascal_connen "/charaktere/pascal-connen"



```
