# Medidas DAX do painel

Medidas principais usadas na Pagina 4 do relatorio.

## Cor da variacao (verde se subiu, vermelho se caiu)
```dax
Cor Total =
IF([QoE Sem Atual] - [QoE Sem Anterior] >= 0, "#2EE08A", "#FF4D6D")
```

## Texto da variacao contra a semana anterior
```dax
Seta Total =
VAR a = [QoE Sem Atual]
VAR b = [QoE Sem Anterior]
VAR d = a - b
RETURN
    IF(ISBLANK(a) || ISBLANK(b), "",
        IF(d >= 0, "▲ ", "▼ ") & FORMAT(ABS(d) * 100, "0.00") & " p.p. vs sem. ant.")
```

## Cor do ranking por estado (semaforo)
```dax
Cor Ranking =
IF([Eficiencia] >= 0.935, "#2EE08A",
    IF([Eficiencia] >= 0.93, "#FFC93C", "#FF4D6D"))
```
