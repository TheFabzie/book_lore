# Haus Connen

Familie aus Arden

## Stammbaum

```mermaid

graph TD
%% Haus Connen

subgraph Gen1["Generation I"]
  harold_connen["Harold Connen<br/>(535-601)"]
  maria_connen["Maria Connen<br/>(541-598)"]
end

harold_connen --- e1((Ehe)) --- maria_connen

subgraph Gen2["Generation II"]
  richard_connen["Richard Connen<br/>(567-)"]
  elizah_connen["Elizah Connen<br/>(569-)"]
  caroline_connen["Caroline Connen<br/>(574-)"]
  cathrine_markant["Cathrine Markant<br/>(571-)"]
end

e1 --> richard_connen
e1 --> elizah_connen
e1 --> caroline_connen

richard_connen --- e2((Ehe)) --- cathrine_markant

subgraph Gen3["Generation III"]
  pascal_connen["Pascal Connen<br/>(596-)"]
end

e2 --> pascal_connen

click harold_connen "/charaktere/harold-connen"
click maria_connen "/charaktere/maria-connen"
click richard_connen "/charaktere/richard-connen"
click elizah_connen "/charaktere/elizah-connen"
click caroline_connen "/charaktere/caroline-connen"
click cathrine_markant "/charaktere/cathrine-markant"
click pascal_connen "/charaktere/pascal-connen"


```
