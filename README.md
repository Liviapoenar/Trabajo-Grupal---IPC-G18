# Trabajo-Grupal---IPC-G18

## Propósito del Trabajo.
Realizar un análisis de las variables implicadas en el contexto de salud, enfermedad y respuesta biológica. 

## Objetivos:
+ Estudiar las distintas variables representadas en la Tabla que se encuentra en [Dataset_expresión_genes](https://github.com/juanfer05/Trabajo-Grupal---IPC-G18/blob/main/Dataset_expresi%C3%B3n_genes_Q11CTnn.csv).
+ Ver la relación que podemos encontrar entre la información demográfica, clínica, sintomatológica, bioquímica, inmunológica y los datos de expresión génica. 
+ Comparación entre individuos con respecto a los resultados obtenidos.

***

## Instrucciones del uso.

Contenido de la Tabla de datos.

### 1. Identificadores de la muestra.
<img width="581" height="62" alt="Captura de pantalla 2026-04-18 234751" src="https://github.com/user-attachments/assets/6ce27dd8-7ac7-4bcd-8e26-a2449754615c" />

### 2. Variables demográficas.

`Edad` edad del individuo expresada en años, *variable continua*.

`Sexo` sexo biológico del individuo, *variable categórica*.

`Exfumador` indica si el individuo ha sido fumador en el pasado, *0= no ; 1=sí* 

### 3. Variables clínicas.

Variables binarias que indican presencia (1) o ausencia (0) de condiciones médicas:

-  **hta:** hipertensión arterial.
-  **dm:** diabetes mellitus. 
-  **alergia:** presencia de enfermedades alérgicas. 
-  **cardiopatia:** enfermedades cardiovasculares. 
-  **ETE:** enfermedad tromboembólica. 
-  **neumopatia:** enfermedades pulmonares. 
-  **hepatopatia:** enfermedades hepáticas. 
-  **colelitiasis:** presencia de cálculos biliares.
-  **utolitiasis:** cálculos urinarios. 
-  **ITU:** infección del tracto urinario. 
-  **renal:** enfermedad renal. 
-  **neuropatia:** trastornos neurológicos. 
-  **corticoides:** uso de medicamentos corticosteroides.

  
### 4. Variables sintomatológicas.

Variables que representan síntomas clínicos reportados (0 = no, 1 = sí):

    • tos: presencia de tos. 
    • disnea: dificultad respiratoria. 
    • expect: expectoración. 
    • secrecion: secreciones respiratorias. 
    • dolor_garg: dolor de garganta. 
    • escalofrios: escalofríos. 
    • fiebre: fiebre. 
    • diarrea: diarrea. 
    • nauseas: náuseas. 
    • vomitos: vómitos. 
    • cefalea: dolor de cabeza. 
    • mareo: mareos. 
    • cansancio: fatiga o debilidad. 
    • anosmia: pérdida del olfato. 
    • disgueusia: alteración del gusto. 
    • dolor_hueso: dolor óseo. 
    • dolor_abdo: dolor abdominal. 
    • perd_ape: pérdida del apetito. 

    
### 5. Variables bioquímicas y hematológicas. 

Variables numéricas que reflejan parámetros clínicos medidos en laboratorio:

| Variable | Descripción |
| --- | --- |
| Glucosa | Nivel de glucosa en sangre |
| Leucocitos | Conteo de glóbulos blancos |
| Linfocitos | Proporción o conteo de linfocitos |
| Neutrofilos | Proporción o conteo de neutrófilos |
| Score_dieta | Índice de calidad de la dietGlucosa. |
| chol | Colesterol total. |
| hdl | Colesterol HDL (colesterol “bueno”) |
| ldl | Colesterol LDL (colesterol “malo”) |
| Trigliceridos | Niveles de triglicéridos |
| Hierro | Concentración de hierro |
| Transferrina | Proteína transportadora de hierro |
| pcr | Proteína C reactiva (indicador de inflamación) |
| cpk | Creatina fosfoquinasa (indicador muscular) |

### 6. Variables inmunológicas. 

-   *igA:* inmunoglobulina A. 
-   *igE:* inmunoglobulina E. 
-   *igE:* inmunoglobulina E. 
-   *igG:* inmunoglobulina G. 
-   *igN:* inmunoglobulina N (posiblemente IgM o variable específica del dataset).

### 7. Variables de calidad de vida.


`calidad_fisica:` percepción de salud física. 

`calidad_mental:` percepción de salud mental. 

### 8. Variables relacionadas con enfermedad tumor
<img width="364" height="87" alt="Captura de pantalla 2026-04-19 004943" src="https://github.com/user-attachments/assets/4bd49625-77b4-4b42-af39-0cd482eeb5ee" />

### 9. Variables de expresión génica.

Las variables que comienzan con el prefijo “AQ_” representan niveles de expresión génica cuantificados. El prefijo “AQ” puede interpretarse como “Absolute Quantification” (cuantificación absoluta).

Cada una corresponde a un gen específico:

| **Genes relacionados con metabolismo y energía** | **Genes inflamatorios e inmunológicos** | **Regulación genética y señalización** | **Estrés oxidativo** | **Inmunorregulación y cáncer** | **Otros genes relevantes** |
| --- | --- | --- | --- | --- | --- |
|       AQ_G6PD: metabolismo de glucosa. | AQ_TNF: factor de necrosis tumoral (inflamación). | AQ_JAK1, AQ_JAK3: señalización celular. | AQ_SOD1: defensa antioxidante. | AQ_PDCD1: regulación inmunológica (PD-1). | AQ_ADIPOQ: metabolismo energético.  | 
AQ_LDHA: metabolismo anaeróbico.  |   AQ_IL6, AQ_IL1B, AQ_IL10: interleucinas (respuesta inmune). | AQ_STAT3: regulación de transcripción. | AQ_GPX1: eliminación de radicales libres. | AQ_CD274: evasión inmune (PD-L1). | AQ_PPARG: regulación metabólica. | 
 AQ_SLC2A4: transporte de glucosa. | AQ_IFNG: interferón gamma. | AQ_MAPK1: señalización celular. | AQ_NFE2L2: regulación antioxidante. | AQ_FOXP3: regulación de células T. | AQ_TGFB1: crecimiento celular. | 
 AQ_CPT1A: metabolismo de lípidos. | AQ_TLR3, AQ_TLR4: receptores tipo Toll (inmunidad innata).  | | | | AQ_CCL2, AQ_CCL5: quimiocinas. | 
 AQ_FASN: síntesis de ácidos grasos. | AQ_NFKB1: regulación inflamatoria.| | | | AQ_CCR5: receptor inmunológico. |

***

> [!NOTE]
> Para más información puede acceder a la siguiente [Carpeta](https://github.com/Liviapoenar/Trabajo-Grupal---IPC-G18/tree/main/scripts).
