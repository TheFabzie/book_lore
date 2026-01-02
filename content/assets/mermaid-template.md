graph TD
%% =====================================
%%  HAUS / FAMILIE: <Name einsetzen>
%% =====================================

%% ---------- Generation I ----------
subgraph Gen1["Generation I"]
  g1_vater["Vorname Nachname"]
  g1_mutter["Vorname Nachname"]
end

g1_vater --- e1((⚭)) --- g1_mutter

%% ---------- Generation II ----------
subgraph Gen2["Generation II"]
  g2_kind1["Vorname Nachname"]
  g2_kind2["Vorname Nachname"]
end

e1 --> g2_kind1
e1 --> g2_kind2

%% ---------- Generation III ----------
subgraph Gen3["Generation III"]
  g3_kind1["Vorname Nachname"]
end

g2_kind1 --- e2((⚭)) --- g2_partner1["Partner Name"]
e2 --> g3_kind1

%% ---------- Klickbare Links ----------
click g1_vater "/personen/dateiname"
click g1_mutter "/personen/dateiname"
click g2_kind1 "/personen/dateiname"
click g2_kind2 "/personen/dateiname"
click g2_partner1 "/personen/dateiname"
click g3_kind1 "/personen/dateiname"
