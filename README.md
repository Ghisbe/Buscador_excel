# Buscador_excel

Este proyecto es un ejercicio práctico de automatización y organización de datos a partir de un archivo PDF, convertido y tratado en Excel, con el objetivo de crear un buscador interactivo de empresas tecnológicas.

La base de datos fue generada con ChatGPT para simular consultas reales de clientes.

<img width="688" height="141" alt="image" src="https://github.com/user-attachments/assets/4fdbe08d-bc82-4fb5-abb4-5368f36bdf6a" />

Proceso del proyecto:
✅Generación de PDF
Se creó un PDF con 200 registros ficticios de empresas tecnológicas que simulan formularios de contacto o consultas por mail.

✅Conversión PDF → Excel
A través de Power Query en Excel se transformó el PDF en una tabla limpia y estructurada, separando cada campo (empresa, contacto, email, fecha, motivo).

✅Creación de buscador en Excel
Se desarrolló un buscador usando: Controles de formulario (ActiveX), Programador de Excel, Fórmula personalizada para búsqueda parcial:

=SI(B1="";"";FILTRAR(Clientes_consulta[#Todo];ESNUMERO(HALLAR(Buscador!B1;Clientes_consulta[[#Todo];[Empresa]]));"Sin resultados"))

Objetivos del proyecto:

- Practicar transformación de datos desde PDF.
- Aplicar técnicas de automatización en Excel.
- Desarrollar buscadores con lógica condicional y diseño funcional.
- Adaptar herramientas entre entornos (Excel vs Google Sheets).
- Mejorar habilidades orientadas a tareas de data entry y preparación de bases de datos.

Tecnologías y herramientas utilizadas:

- Excel + Power Query
- Controles de formulario (ActiveX).
- ChatGPT (generación de datos).
- YouTube (tutorial base para buscador):
https://www.youtube.com/watch?v=JQjxFpAk0YQ

Próximos pasos:

- Incorporar conexión a base de datos (MySQL o SQLite).
- Automatizar carga masiva desde Excel a SQL.
- Diseñar una interfaz con formularios para nuevas entradas.
