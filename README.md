Lector Interactivo: De Bello GallicoEste es un proyecto educativo diseñado para facilitar el estudio y análisis del texto clásico De Bello Gallico de Julio César. La herramienta está construida como una aplicación web de una sola página, completamente autocontenida en un único archivo index.html, lo que la hace fácil de usar, compartir y modificar.✨ Características PrincipalesLa aplicación ofrece una experiencia de lectura enriquecida con las siguientes funcionalidades interactivas:Texto Interactivo: El texto en latín está dividido en oraciones y palabras. Cada elemento es clicable para obtener un análisis detallado.Análisis Morfológico Instantáneo: Al hacer clic en una palabra, se abre una barra lateral que muestra su análisis morfológico completo en latín, junto con su significado en varios idiomas.Análisis Sintáctico Completo: Al hacer clic en una oración completa, el usuario es llevado a una vista de análisis detallado que incluye:La oración original en latín.Traducciones a múltiples idiomas.Un análisis sintáctico completo de la estructura de la oración.Traducción Rápida (Tooltip): Al pasar el ratón sobre una oración, aparece una ventana emergente con una traducción rápida en el idioma seleccionado por el usuario.Soporte Multilingüe: Las traducciones y el análisis están disponibles en:EspañolInglésChino Tradicional (中文)Coreano (한국어)Interfaz Personalizable: El usuario puede seleccionar su idioma de preferencia para las traducciones rápidas, y esta elección se guarda para futuras sesiones.Diseño No Invasivo: La barra lateral de análisis se desliza sin tapar el texto principal, permitiendo una visualización simultánea del contexto y el análisis.🚀 Cómo UsarHay dos maneras de utilizar esta herramienta:En línea (Recomendado): Simplemente visita la página publicada a través de GitHub Pages en la siguiente URL:[ENLACE A TU PÁGINA DE GITHUB PAGES AQUÍ] (Deberás reemplazar esto con el enlace que GitHub te proporcionó)Localmente:Descarga el archivo index.html de este repositorio.Ábrelo directamente con cualquier navegador web moderno (como Chrome, Firefox, Edge, etc.).🔧 Cómo Modificar o Añadir ContenidoToda la lógica, los estilos y el contenido de la aplicación están dentro del archivo index.html. Para añadir nuevos capítulos o modificar el análisis existente, sigue estos pasos:Abre el archivo index.html con un editor de texto o código.Busca la etiqueta <script> al final del archivo.Dentro del script, localiza la constante const paragrafus.Esta constante contiene un objeto con una lista llamada orationes. Cada elemento de esta lista es un objeto que representa una oración y contiene:id_orationis: Un identificador único para la oración (ej: 'o9').textus_latinus: El texto completo de la oración en latín.translationes: Un objeto con las traducciones (es, en, zh, ko).analysis_syntactica: Un string (puede contener HTML) con el análisis sintáctico.verba: Una lista de objetos, donde cada objeto representa una palabra con su id_verbi, terminus, analysis_morphologicus y significationes.Puedes editar estos objetos o añadir nuevos a la lista orationes para expandir el contenido de la herramienta.const paragrafus = {
    id: 1,
    orationes: [
        {
            id_orationis: 'o1',
            textus_latinus: "...",
            translationes: {
                es: '...',
                en: '...',
                zh: '...',
                ko: '...'
            },
            analysis_syntactica: `...`,
            verba: [
                { 
                    id_verbi: 'v1_1', 
                    terminus: 'Gallia', 
                    /* ... */ 
                },
                /* ... más palabras ... */
            ]
        },
        /* ... más oraciones ... */
    ]
};
📜 FuenteEl texto original en latín es Commentarii de Bello Gallico, escrito por Cayo Julio César. Las traducciones y análisis han sido compilados para este proyecto educativo.Este proyecto fue desarrollado como una herramienta de código abierto para estudiantes y entusiastas de los clásicos.
