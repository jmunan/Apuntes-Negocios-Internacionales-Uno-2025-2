<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Curso: Negocios Internacionales 1</title>
    <style>
        :root {
            --primary-bg-color: #121212;
            --secondary-bg-color: #1e1e1e;
            --primary-text-color: #e0e0e0;
            --accent-color: #bb86fc;
            --border-color: #333333;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
            background-color: var(--primary-bg-color);
            color: var(--primary-text-color);
            margin: 0;
            line-height: 1.6;
        }

        #sidebar {
            height: 100%;
            width: 0;
            position: fixed;
            z-index: 2;
            top: 0;
            left: 0;
            background-color: var(--secondary-bg-color);
            overflow-x: hidden;
            transition: 0.5s;
            padding-top: 60px;
            border-right: 1px solid var(--border-color);
        }

        #sidebar a {
            padding: 10px 15px;
            text-decoration: none;
            font-size: 1.2em;
            color: var(--primary-text-color);
            display: block;
            transition: 0.3s;
        }

        #sidebar a:hover {
            background-color: var(--accent-color);
            color: var(--primary-bg-color);
        }

        #sidebar .closebtn {
            position: absolute;
            top: 0;
            right: 25px;
            font-size: 36px;
            margin-left: 50px;
        }

        #menu-toggle {
            transition: margin-left .5s;
            padding: 16px;
            position: fixed;
            top: 10px;
            left: 10px;
            font-size: 2em;
            cursor: pointer;
            z-index: 1;
            background-color: var(--secondary-bg-color);
            border-radius: 8px;
        }

        #main-content {
            transition: margin-left .5s;
            padding: 20px;
            font-size: 1.8em; /* Large font size for projectors */
        }

        .content-block {
            display: none;
        }

        .content-block.active {
            display: block;
        }

        .collapsible {
            background-color: var(--secondary-bg-color);
            color: var(--primary-text-color);
            cursor: pointer;
            padding: 18px;
            width: 100%;
            border: none;
            text-align: left;
            outline: none;
            font-size: 1.2em;
            margin-top: 15px;
            border-radius: 5px;
            border-left: 5px solid var(--accent-color);
        }

        .collapsible:after {
            content: '\002B'; /* Plus sign */
            font-weight: bold;
            float: right;
            margin-left: 5px;
        }

        .active-collapsible:after {
            content: "\2212"; /* Minus sign */
        }

        .collapsible-content {
            padding: 0 18px;
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.3s ease-out;
            background-color: var(--primary-bg-color);
            font-size: 0.9em;
            border-left: 1px solid var(--border-color);
            border-right: 1px solid var(--border-color);
            border-bottom: 1px solid var(--border-color);
        }
        
        .collapsible-content p, .collapsible-content ul, .collapsible-content h4 {
            margin-top: 15px;
            margin-bottom: 15px;
        }

        h1, h2, h3 {
            color: var(--accent-color);
        }

        h4 {
            font-size: 1.1em;
            color: var(--primary-text-color);
            border-bottom: 1px solid var(--border-color);
            padding-bottom: 5px;
        }

        cite {
            font-style: italic;
            font-size: 0.8em;
            color: #aaa;
            display: block;
            margin-top: 10px;
        }

        ul {
            list-style-type: square;
        }

    </style>
</head>
<body>

<div id="sidebar">
    <a href="javascript:void(0)" class="closebtn" onclick="closeNav()">&times;</a>
    <a href="#" onclick="showContent('bloque1')">Bloque 1: Fundamentos</a>
    <a href="#" onclick="showContent('bloque2')">Bloque 2: Comercio e Inversión</a>
    <a href="#" onclick="showContent('bloque3')">Bloque 3: Ética y Estrategia</a>
    <a href="#" onclick="showContent('referencias')">Referencias</a>
</div>

<div id="main-content">
    <span id="menu-toggle" onclick="openNav()">&#9776; Menú</span>
    
    <div id="welcome" class="content-block active">
        <h1>Curso Interactivo de Negocios Internacionales 1</h1>
        <p>Bienvenido. Esta es una versión nueva y significativamente ampliada del curso, desarrollada para asegurar una cobertura completa y detallada de todos los temas.</p>
        <p>Utilice el menú de la izquierda para navegar por los bloques temáticos. Cada tema principal es un botón desplegable; haga clic en él para revelar el contenido exhaustivo.</p>
    </div>

    <!-- BLOQUE TEMÁTICO 1 -->
    <div id="bloque1" class="content-block">
        <h2>Primer Bloque Temático</h2>

        <button class="collapsible">Fundamentos de los Negocios Internacionales</button>
        <div class="collapsible-content">
            <h4>Definición y Alcance</h4>
            <p>Los negocios internacionales comprenden todas las transacciones comerciales —incluyendo el comercio de bienes y servicios, las inversiones, y el transporte— que se realizan a través de las fronteras nacionales. Involucra a dos o más países y puede ser llevado a cabo tanto por empresas privadas como por entidades gubernamentales (Daniels et al., 2013). El estudio de este campo no solo se enfoca en las grandes Empresas Multinacionales (EMN), sino también en las Pequeñas y Medianas Empresas (PYMES), que cada vez más participan en la arena global.</p>

            <h4>Globalización: Un Mundo Interconectado</h4>
            <p>La globalización se refiere al cambio hacia una economía mundial más integrada e interdependiente. Es un proceso que erosiona las barreras económicas, culturales y tecnológicas que antes separaban a las naciones.</p>
            <ul>
                <li><b>Globalización de los mercados:</b> Es la fusión de mercados nacionales, históricamente distintos y separados, en un único mercado mundial. La convergencia de gustos y preferencias de los consumidores, impulsada por marcas globales, facilita esta tendencia. Sin embargo, es importante no exagerar; todavía existen diferencias significativas entre los mercados nacionales que requieren adaptación (Hill, 2021).</li>
                <li><b>Globalización de la producción:</b> Consiste en la subcontratación de bienes y servicios en diversas ubicaciones del mundo para aprovechar las diferencias en el costo y la calidad de los factores de producción (mano de obra, energía, capital). El objetivo es reducir costos y mejorar la calidad para competir eficazmente. Un ejemplo paradigmático es el Boeing 787, con componentes provenientes de más de una docena de países.</li>
            </ul>

            <h4>Impulsores Clave de la Globalización</h4>
            <p>Dos factores interrelacionados han impulsado la globalización:</p>
            <ol>
                <li><b>Disminución de las barreras al comercio y la inversión:</b> Después de la Segunda Guerra Mundial, las naciones avanzadas se comprometieron a reducir las barreras. Bajo el Acuerdo General sobre Aranceles Aduaneros y Comercio (GATT) y posteriormente la Organización Mundial del Comercio (OMC), se han reducido drásticamente los aranceles y otras barreras, facilitando el comercio transfronterizo.</li>
                <li><b>El papel del cambio tecnológico:</b> Los avances en microprocesadores y telecomunicaciones, la aparición de Internet y el desarrollo de la logística y el transporte han sido fundamentales. Internet ha democratizado el comercio global, permitiendo a pequeñas empresas llegar a clientes en todo el mundo. La contenedorización ha reducido radicalmente los costos y tiempos del transporte marítimo, convirtiéndolo en un método altamente eficiente.</li>
            </ol>

            <h4>El Debate sobre la Globalización: Pros y Contras</h4>
            <p>La globalización es un fenómeno complejo con efectos diversos, lo que genera un intenso debate:</p>
            <ul>
                <li><b>A favor:</b> Los defensores argumentan que la especialización y el comercio aumentan la eficiencia económica mundial, reducen los precios para los consumidores, estimulan el crecimiento económico, crean empleos y ayudan a sacar a los países de la pobreza.</li>
                <li><b>En contra:</b> Los críticos sostienen que la globalización provoca la pérdida de empleos en los países desarrollados a medida que las empresas se trasladan a países con salarios más bajos. También expresan preocupaciones sobre la degradación ambiental, la explotación laboral en una "carrera hacia el fondo" y la pérdida de soberanía nacional y cultural.</li>
            </ul>
            <cite>Fuentes: Hill (2021), Daniels et al. (2013), Peng (2012).</cite>
        </div>

        <button class="collapsible">Ámbitos Culturales de las Empresas</button>
        <div class="collapsible-content">
            <h4>La Importancia de la Cultura</h4>
            <p>La cultura es un sistema complejo de valores (lo que un grupo considera bueno o deseable) y normas (las reglas sociales que rigen el comportamiento) que están interrelacionados y forman un diseño para vivir. La conciencia intercultural y la competencia cultural ya no son un lujo, sino una necesidad fundamental para los gerentes internacionales.</p>

            <h4>Determinantes de la Cultura</h4>
            <p>La cultura de una sociedad se forma a partir de varios factores:</p>
            <ul>
                <li><b>Estructura social:</b> La organización básica de una sociedad, incluyendo el grado en que se enfatiza el individuo frente al grupo (individualismo vs. colectivismo) y la estratificación social.</li>
                <li><b>Lenguaje:</b> Es el vehículo de la cultura, tanto hablado como no hablado (lenguaje corporal). Un error de traducción puede tener consecuencias desastrosas.</li>
                <li><b>Religión y Sistemas Éticos:</b> Proporcionan un marco moral y de valores que puede influir profundamente en las prácticas comerciales, desde las horas de trabajo hasta los tipos de productos que se pueden consumir.</li>
                <li><b>Educación:</b> El sistema educativo de un país juega un papel clave en la transmisión de conocimientos, habilidades y valores culturales.</li>
            </ul>

            <h4>Marco Cultural de Hofstede</h4>
            <p>El marco de Geert Hofstede es la herramienta más utilizada para analizar las diferencias culturales:</p>
            <ul>
                <li><b>Distancia al poder:</b> Alta en países como Malasia, donde se aceptan las jerarquías; baja en países como Dinamarca, donde se prefiere la igualdad.</li>
                <li><b>Individualismo vs. Colectivismo:</b> EE.UU. es altamente individualista; Guatemala es fuertemente colectivista.</li>
                <li><b>Aversión a la incertidumbre:</b> Alta en Grecia, donde se prefieren reglas claras; baja en Singapur, donde se tolera la ambigüedad.</li>
                <li><b>Masculinidad vs. Feminidad:</b> Japón es una cultura "masculina" (competitiva); Suecia es "femenina" (enfocada en la calidad de vida).</li>
                <li><b>Orientación a largo plazo:</b> Alta en países asiáticos como Japón, que valoran el ahorro y la perseverancia.</li>
            </ul>

            <h4>Caso de Estudio: La Adaptación de McDonald's</h4>
            <p>McDonald's es un maestro de la adaptación cultural. Mientras que su modelo de negocio y su marca son globales, su menú se adapta a los gustos locales. En la India, donde la vaca es sagrada, no se sirve carne de res. En su lugar, ofrecen la McAloo Tikki Burger (una hamburguesa de patata y guisantes) y la Maharaja Mac (hecha con pollo). Este es un ejemplo perfecto de cómo equilibrar la estandarización global con la adaptación local.</p>
            <cite>Fuentes: Hill (2021), Peng (2012).</cite>
        </div>

        <button class="collapsible">Ámbito Político y Legal de las Empresas</button>
        <div class="collapsible-content">
            <h4>Sistemas Políticos, Económicos y Legales</h4>
            <p>Estos tres sistemas están interconectados y su configuración afecta profundamente el atractivo de un país como mercado o sitio de inversión.</p>
            <ul>
                <li><b>Sistemas Políticos:</b> Se evalúan en dos dimensiones: el grado de colectivismo vs. individualismo, y el grado de democracia vs. totalitarismo.</li>
                <li><b>Sistemas Económicos:</b> Varían desde economías de mercado puras (impulsadas por la oferta y la demanda), pasando por economías mixtas (con un sector público y privado significativo), hasta economías de mando (donde el gobierno planifica y controla la actividad económica).</li>
                <li><b>Sistemas Legales:</b> Se refieren a las reglas que regulan el comportamiento. Los principales son el Derecho Común (Common Law, basado en precedentes, como en EE.UU.), el Derecho Civil (basado en códigos detallados, como en Francia o México) y el Derecho Teocrático (basado en doctrina religiosa, como la Sharia en algunos países islámicos).</li>
            </ul>

            <h4>Riesgo Político y Legal</h4>
            <p>El riesgo político es la probabilidad de que fuerzas políticas causen cambios drásticos en el entorno empresarial de un país. El riesgo legal es la probabilidad de que un socio comercial rompa un contrato o expropie derechos de propiedad. La protección de los derechos de propiedad, incluyendo la propiedad intelectual (PI), es un tema crítico.</p>
            <ul>
                <li><b>Propiedad Intelectual:</b> Se refiere a la propiedad que es producto de la actividad intelectual. Se protege mediante:
                    <ul>
                        <li><b>Patentes:</b> Derechos exclusivos para un nuevo producto o proceso.</li>
                        <li><b>Derechos de autor:</b> Protección para obras creativas (libros, música, software).</li>
                        <li><b>Marcas:</b> Nombres y logotipos que identifican a un producto o empresa.</li>
                    </ul>
                </li>
            </ul>
            <p>La piratería de PI es un problema grave. Organizaciones como la Organización Mundial de la Propiedad Intelectual (OMPI) y acuerdos como TRIPS de la OMC buscan armonizar y fortalecer la protección a nivel mundial.</p>
            <cite>Fuentes: Hill (2021), Daniels et al. (2013).</cite>
        </div>
    </div>

    <!-- BLOQUE TEMÁTICO 2 -->
    <div id="bloque2" class="content-block">
        <h2>Segundo Bloque Temático</h2>

        <button class="collapsible">Teoría del Comercio Internacional</button>
        <div class="collapsible-content">
            <h4>Mercantilismo (Siglo XVI-XVIII)</h4>
            <p>El mercantilismo abogaba por que un país debía maximizar sus exportaciones y minimizar sus importaciones para acumular oro y plata, lo que se consideraba la base de la riqueza nacional. Veía el comercio como un "juego de suma cero", donde la ganancia de un país se producía a expensas de otro. Aunque intelectualmente obsoleto, su retórica proteccionista (neomercantilismo) sigue viva.</p>

            <h4>Ventaja Absoluta (Adam Smith, 1776)</h4>
            <p>En su obra "La Riqueza de las Naciones", Adam Smith atacó el mercantilismo y defendió el libre comercio. Argumentó que un país tiene una <b>ventaja absoluta</b> en la producción de un bien cuando es más eficiente (utiliza menos recursos) que cualquier otro país para producirlo. Según Smith, los países no deben producir bienes que pueden comprar a menor costo a otros. Deberían especializarse en la producción de bienes en los que tienen una ventaja absoluta y comerciar entre sí. Esto crea un "juego de suma positiva" donde ambos países se benefician.</p>

            <h4>Ventaja Comparativa (David Ricardo, 1817)</h4>
            <p>David Ricardo llevó la teoría de Smith un paso más allá. Demostró que el comercio es beneficioso incluso si un país tiene una ventaja absoluta en la producción de todos los bienes. Lo que importa es la <b>ventaja comparativa</b>, es decir, la eficiencia relativa. Un país debe especializarse en producir el bien en el que es relativamente más eficiente (o donde su desventaja absoluta es menor) e importar los demás. Esta teoría se basa en el concepto de costo de oportunidad y es la base intelectual del libre comercio moderno.</p>

            <h4>Teorías Modernas del Comercio</h4>
            <ul>
                <li><b>Teoría de Heckscher-Ohlin:</b> La ventaja comparativa surge de las diferencias en las dotaciones de factores de un país (tierra, trabajo, capital). Los países exportan bienes que utilizan intensivamente sus factores abundantes.</li>
                <li><b>Teoría del Ciclo de Vida del Producto (Vernon):</b> A medida que los productos maduran, su producción se traslada de países desarrollados a países en desarrollo, alterando los patrones de comercio.</li>
                <li><b>Nueva Teoría del Comercio (Krugman):</b> En industrias con economías de escala, el comercio permite aumentar la variedad de productos y reducir los costos. También introduce el concepto de "ventaja del primer jugador".</li>
                <li><b>Diamante de Porter:</b> Explica la competitividad nacional en ciertas industrias basándose en cuatro atributos: condiciones de los factores, condiciones de la demanda, industrias relacionadas y de apoyo, y estrategia, estructura y rivalidad de la empresa.</li>
            </ul>
            <cite>Fuentes: Hill (2021), Peng (2012), Daniels et al. (2013).</cite>
        </div>

        <button class="collapsible">La Influencia Gubernamental en el Comercio</button>
        <div class="collapsible-content">
            <h4>Instrumentos de Política Comercial</h4>
            <p>Los gobiernos utilizan siete instrumentos principales para intervenir en el comercio:</p>
            <ol>
                <li><b>Aranceles:</b> Impuestos sobre las importaciones. Elevan el costo para los importadores y los precios para los consumidores.</li>
                <li><b>Subsidios:</b> Pagos del gobierno a los productores nacionales para ayudarles a competir.</li>
                <li><b>Cuotas de Importación:</b> Restricción cuantitativa directa sobre la importación de un bien.</li>
                <li><b>Restricciones Voluntarias a la Exportación (RVE):</b> Cuotas impuestas por el país exportador, generalmente a petición del importador.</li>
                <li><b>Requisitos de Contenido Local:</b> Obligación de que una fracción de un bien se produzca localmente.</li>
                <li><b>Políticas Administrativas:</b> Reglas burocráticas diseñadas para dificultar la entrada de importaciones.</li>
                <li><b>Políticas Antidumping:</b> Aranceles punitivos contra la venta de bienes importados por debajo de su costo de producción ("dumping").</li>
            </ol>

            <h4>Argumentos para la Intervención Gubernamental</h4>
            <p>Los argumentos se dividen en políticos y económicos:</p>
            <ul>
                <li><b>Argumentos Políticos:</b> Se centran en proteger los intereses de ciertos grupos, a menudo a expensas de otros. Incluyen la protección de empleos, la seguridad nacional, las represalias, la protección de los consumidores y la promoción de objetivos de política exterior.</li>
                <li><b>Argumentos Económicos:</b> Buscan aumentar la riqueza total de una nación. Incluyen el "argumento de la industria naciente" (proteger a las industrias nuevas hasta que sean viables) y la "política comercial estratégica" (ayudar a las empresas nacionales a obtener ventajas de primer jugador en industrias clave).</li>
            </ul>
            <cite>Fuentes: Hill (2021), Daniels et al. (2013).</cite>
        </div>

        <button class="collapsible">La Inversión Extranjera Directa (IED)</button>
        <div class="collapsible-content">
            <h4>Definición y Formas de IED</h4>
            <p>La IED ocurre cuando una empresa invierte directamente en instalaciones para producir o comercializar un producto en un país extranjero, adquiriendo un interés de control. Las dos formas son:</p>
            <ul>
                <li><b>Inversión Greenfield:</b> Construir una operación desde cero.</li>
                <li><b>Adquisición o Fusión:</b> Comprar o fusionarse con una empresa local. Las adquisiciones son más rápidas pero pueden presentar desafíos de integración.</li>
            </ul>

            <h4>Teorías de la IED: ¿Por qué Invertir en lugar de Exportar o Licenciar?</h4>
            <p>La IED se prefiere cuando existen imperfecciones en el mercado. Las principales teorías son:</p>
            <ul>
                <li><b>Teoría de la Internalización:</b> Explica que las empresas eligen la IED para evitar las desventajas de la concesión de licencias, como el riesgo de perder control sobre su tecnología o su know-how.</li>
                <li><b>Paradigma Ecléctico de Dunning (OLI):</b> Sostiene que la IED es ventajosa cuando se combinan tres factores: <b>Ventajas de Propiedad</b> (un activo único como una marca o tecnología), <b>Ventajas de Localización</b> (recursos o mercados atractivos en el extranjero) y <b>Ventajas de Internalización</b> (beneficios de controlar la operación directamente).</li>
            </ul>

            <h4>Beneficios y Costos de la IED</h4>
            <p>La IED tiene un impacto significativo tanto en el país anfitrión (receptor) como en el de origen.</p>
            <ul>
                <li><b>País Anfitrión (Receptor):</b><br><b>Beneficios:</b> Transferencia de recursos (capital, tecnología), creación de empleo, mejora de la balanza de pagos, aumento de la competencia y crecimiento económico.<br><b>Costos:</b> Efectos adversos sobre la competencia local, posible salida de ganancias que afecta la balanza de pagos, y preocupaciones sobre la soberanía nacional.</li>
                <li><b>País de Origen:</b><br><b>Beneficios:</b> Entrada de divisas por las ganancias repatriadas, aumento de las exportaciones de componentes, y aprendizaje de nuevas habilidades y tecnologías.<br><b>Costos:</b> Salida de capital y posible pérdida de empleos si la producción en el extranjero sustituye a la nacional.</li>
            </ul>
            <cite>Fuentes: Hill (2021), Peng (2012).</cite>
        </div>
    </div>

    <!-- BLOQUE TEMÁTICO 3 -->
    <div id="bloque3" class="content-block">
        <h2>Tercer Bloque Temático</h2>

        <button class="collapsible">Problemas Éticos y Responsabilidad Social</button>
        <div class="collapsible-content">
            <h4>Dilemas Éticos en los Negocios Internacionales</h4>
            <p>Los problemas éticos más comunes en los negocios internacionales se refieren a: prácticas de empleo, derechos humanos, normas medioambientales, corrupción y la obligación moral de las empresas multinacionales.</p>

            <h4>Las Raíces del Comportamiento Poco Ético</h4>
            <p>Las razones por las que los gerentes pueden comportarse de manera poco ética incluyen: la ética personal, procesos de toma de decisiones que no consideran la ética, una cultura organizacional que no valora la ética, metas de desempeño poco realistas que presionan a los gerentes, y un liderazgo poco ético.</p>

            <h4>Enfoques Filosóficos sobre la Ética</h4>
            <p>Para guiar la toma de decisiones, los gerentes pueden recurrir a varios marcos filosóficos:</p>
            <ul>
                <li><b>Los "Hombres de Paja":</b> Argumentos a menudo utilizados pero deficientes. Incluyen la Doctrina Friedman, el relativismo cultural y el moralista justo.</li>
                <li><b>Enfoques Sólidos:</b><br><b>Utilitarismo:</b> Se centra en las consecuencias; la mejor decisión es la que produce el mayor bien para el mayor número de personas.<br><b>Ética Kantiana:</b> Se basa en la idea de que las personas tienen dignidad y deben ser tratadas como fines, no como medios.<br><b>Teorías de los Derechos:</b> Sostienen que los seres humanos tienen derechos y privilegios fundamentales que trascienden las fronteras nacionales.<br><b>Teorías de la Justicia:</b> Proponen una distribución justa de los bienes y servicios económicos (por ejemplo, el velo de la ignorancia de Rawls).</li>
            </ul>

            <h4>Caso: La Ley de Prácticas Corruptas en el Extranjero (FCPA) de EE.UU.</h4>
            <p>Esta ley prohíbe a las empresas estadounidenses sobornar a funcionarios de gobiernos extranjeros para obtener o mantener negocios. La ley permite los "pagos de facilitación" (pequeños pagos para acelerar trámites rutinarios), pero la línea a menudo es borrosa, creando un dilema ético para los gerentes.</p>
            <cite>Fuentes: Hill (2021), Peng (2012).</cite>
        </div>

        <button class="collapsible">El Uso de Divisas</button>
        <div class="collapsible-content">
            <h4>Funciones del Mercado de Divisas (Forex)</h4>
            <p>El mercado de divisas es fundamental para los negocios internacionales. Sus funciones clave son:</p>
            <ol>
                <li><b>Conversión de divisas:</b> Permite a las empresas convertir los ingresos, pagar a los proveedores y realizar inversiones en diferentes monedas.</li>
                <li><b>Proporcionar cobertura contra el riesgo cambiario:</b> El riesgo cambiario es el que se deriva de las variaciones adversas de los tipos de cambio. El mercado ofrece instrumentos como los contratos a plazo (forwards) y las opciones para gestionar este riesgo.</li>
            </ol>

            <h4>Determinación de los Tipos de Cambio</h4>
            <p>Los tipos de cambio se determinan por la demanda y la oferta de diferentes monedas. Tres factores principales influyen en los movimientos futuros del tipo de cambio:</p>
            <ul>
                <li><b>La Ley del Precio Único y la Paridad del Poder Adquisitivo (PPA):</b> La PPA sugiere que, a largo plazo, los tipos de cambio se mueven para igualar los precios de una canasta idéntica de bienes y servicios entre países. La inflación es un motor clave de esto.</li>
                <li><b>Tasas de Interés:</b> El Efecto Fisher establece que las tasas de interés nominales de un país reflejan las expectativas de inflación. El Efecto Fisher Internacional sugiere que el tipo de cambio al contado debería cambiar en una cantidad igual pero en dirección opuesta a la diferencia en las tasas de interés nominales entre dos países.</li>
                <li><b>Psicología del Mercado:</b> Las expectativas de los inversores y los efectos de arrastre (bandwagon effects) pueden causar movimientos a corto plazo que no se basan en los fundamentos económicos.</li>
            </ul>
            <cite>Fuentes: Hill (2021), Daniels et al. (2013).</cite>
        </div>

        <button class="collapsible">Empresas Multinacionales (EMN)</button>
        <div class="collapsible-content">
            <h4>El Reto Estratégico de las EMN</h4>
            <p>Las EMN se enfrentan a dos presiones competitivas opuestas: la <b>presión por la reducción de costos</b> (que impulsa la estandarización global) y la <b>presión por la adaptación local</b> (que impulsa la personalización de productos y estrategias para cada mercado).</p>

            <h4>Cuatro Estrategias Básicas</h4>
            <p>La forma en que una empresa responde a estas presiones determina su estrategia:</p>
            <ol>
                <li><b>Estrategia de Estandarización Global:</b> Alto enfoque en la reducción de costos, bajo en la adaptación local. Se centraliza la producción en ubicaciones óptimas. <b>Ejemplo:</b> Intel, produciendo microprocesadores estandarizados para un mercado mundial.</li>
                <li><b>Estrategia de Localización:</b> Bajo enfoque en costos, alto en adaptación local. Se personalizan productos y marketing para cada país. <b>Ejemplo:</b> MTV, que solía tener una programación muy localizada para cada región.</li>
                <li><b>Estrategia Transnacional:</b> Alto enfoque en costos y en adaptación local simultáneamente. Es la más difícil de lograr. Busca un flujo multidireccional de habilidades y productos entre todas las subsidiarias. <b>Ejemplo:</b> Ford, con su estrategia "One Ford", intenta diseñar coches globales que puedan ser adaptados a diferentes mercados.</li>
                <li><b>Estrategia Internacional:</b> Bajo enfoque en costos y en adaptación local. A menudo para empresas con productos únicos y poca competencia. <b>Ejemplo:</b> Microsoft en sus inicios, exportando su sistema operativo estándar.</li>
            </ol>

            <h4>Arquitectura Organizacional</h4>
            <p>Para que la estrategia funcione, la arquitectura de la EMN debe ser coherente. Esto incluye:
            <ul>
                <li><b>Estructura:</b> La división formal de la organización (por ejemplo, por producto, por área geográfica).</li>
                <li><b>Sistemas de Control:</b> Las métricas utilizadas para medir el desempeño.</li>
                <li><b>Incentivos:</b> Los dispositivos utilizados para recompensar el comportamiento directivo adecuado.</li>
                <li><b>Procesos, Cultura y Personal:</b> Los demás elementos que conforman la forma de trabajar de la organización.</li>
            </ul>
            <cite>Fuentes: Hill (2021), Peng (2012).</cite>
        </div>
    </div>
    
    <!-- REFERENCIAS -->
    <div id="referencias" class="content-block">
        <h2>Referencias Bibliográficas</h2>
        <p>El contenido de este curso ha sido sintetizado a partir de las siguientes obras, de acuerdo con las normas de citación APA.</p>
        
        <p>Daniels, J., Radebaugh, L., & Sullivan, D. (2013). <i>Negocios internacionales: Ambientes y operaciones</i> (14a ed.). Pearson Educación.</p>
        
        <p>Hill, C. W. L. (2021). <i>Negocios internacionales: Competencia en el mercado global</i> (12a ed.). McGraw-Hill Interamericana.</p>
        
        <p>Peng, M. W. (2012). <i>Negocios globales</i> (2a. ed.). Cengage Learning.</p>
    </div>

</div>

<script>
    function openNav() {
        document.getElementById("sidebar").style.width = "250px";
        document.getElementById("main-content").style.marginLeft = "250px";
    }

    function closeNav() {
        document.getElementById("sidebar").style.width = "0";
        document.getElementById("main-content").style.marginLeft = "0";
    }

    function showContent(blockId) {
        var contentBlocks = document.getElementsByClassName("content-block");
        for (var i = 0; i < contentBlocks.length; i++) {
            contentBlocks[i].classList.remove("active");
        }
        document.getElementById(blockId).classList.add("active");
        if (window.innerWidth <= 768) { // Close nav on selection on mobile
            closeNav();
        }
    }

    var coll = document.getElementsByClassName("collapsible");
    for (var i = 0; i < coll.length; i++) {
        coll[i].addEventListener("click", function() {
            this.classList.toggle("active-collapsible");
            var content = this.nextElementSibling;
            if (content.style.maxHeight){
                content.style.maxHeight = null;
            } else {
                content.style.maxHeight = content.scrollHeight + "px";
            } 
        });
    }
    
    // Show welcome message by default
    document.getElementById('welcome').classList.add('active');

</script>

</body>
</html>
