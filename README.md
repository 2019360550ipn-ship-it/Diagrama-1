# Diagrama-1
# Mi Diagrama de Proceso

```mermaid
graph TD
    MuelleDescarga[MUELLE DE DESCARGA<br/>Entrada MP] --> AlmacenMP
    MuelleCarga[MUELLE DE CARGA<br/>Salida PT] <-- AlmacenPT
    AlmacenMP[ALMACÉN MATERIA PRIMA<br/>Rollos de Acero]
    AlmacenPT[ALMACÉN PROD. TERMINADO<br/>Cajas / Pallets]
    
    AlmacenMP --> Proceso1[1. DECAPADO Y PREP.]
    Proceso1 --> Proceso2[2. PRENSAS FORMADO]
    Proceso2 --> Proceso3[3. ROSCADO (LAMINADO)]
    Proceso3 --> Proceso4[4. HORNOS TRAT. TÉRMICO]
    Proceso3 --> Proceso5[5. RECUBRIMIENTO<br/>(Galvanizado)]
    Proceso4 --> Proceso6[6. LABORATORIO]
    Proceso6 --> Proceso5
    Proceso5 --> Proceso7[7. EMPAQUE]
    Proceso7 --> AlmacenPT
    
    style Proceso2 fill:#f9f,stroke:#333,stroke-width:2px
```
