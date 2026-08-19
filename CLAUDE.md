# Reglas de trabajo

Take home de Backend/DevOps. Django + Ninja + Postgres 16.
Trabajamos por bloques. No avances al siguiente sin que yo lo diga.

## Metodo
- Toda afirmacion de performance requiere evidencia en bench/.
- Antes de proponer un fix, muestrame el EXPLAIN que lo justifica.
- Mediciones siempre con DEBUG=False.
- Latencia y conteo de queries se miden en corridas separadas.
- No cambiar el hosting de Postgres entre baseline y re-medicion.

## Bloques
- 0 baseline: prohibido modificar codigo de aplicacion, solo medicion.
- 1 diagnostico: instrumentacion y tabla de queries por endpoint.
- 2 fixes: un commit por arreglo, con numeros antes/despues en el mensaje.
- 3 re-medicion.
- 4 developer experience.
- 5 produccion.
- 6 NOTES.md.
- 7 revision adversarial.

## Alcance cerrado
- No implementar auth.
- No redisenar el modelo de dominio.
- No agregar abstracciones ni comentarios explicativos de mas.
- No tocar bench/baseline/ despues de congelado.
