# Haus Connen

Familie aus Arden

## Stammbaum

graph TD
%% =====================================
%%  HAUS / FAMILIE: <Connen>
%% =====================================

%% ---------- Generation I ----------
subgraph Gen1["Generation I"]
  harold-connen["✝ Harold Connen<br/>(535–601)"]
  maria-connen["✝ Maria Connen<br/>(541–598)"]
end

harold-connen --- e1((⚭)) --- maria-connen

%% ---------- Generation II ----------
subgraph Gen2["Generation II"]
  richard-connen["* Richard Connen<br/>(567–)"]
  elizah-connen["Elizah Connen<br/>(569–)"]
  caroline-connen["Caroline Connen<br/>(574–)"]
  cathrine-markant["Cathrine Markant<br/>(571–)"]
end

e1 --> richard-connen
e1 --> elizah-connen
e1 --> caroline-connen


%% ---------- Generation III ----------
subgraph Gen3["Generation III"]
  pascal-connen["Pascal Connen<br/>(596–)"]
end

richard-connen --- e2((⚭)) --- cathrine-markant
e2 --> pascal-connen

%% ---------- Klickbare Links ----------
click harold-connen "/charaktere/harold-connen"
click maria-connen "/charaktere/maria-connen"
click richard-connen "/charaktere/richard-connen"
click elizah-connen "/charaktere/elizah-connen"
click caroline-connen "/charaktere/caroline-connen"
click cathrine-markant "/charaktere/cathrine-markant"
click pascal-connen "/charaktere/pascal-connen"
