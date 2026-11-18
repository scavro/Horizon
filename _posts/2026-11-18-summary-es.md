---
layout: default
title: "Horizon Summary: 2026-11-18 (ES)"
date: 2026-11-18
lang: es
---

> De 71 elementos analizados, se seleccionaron 7 noticias relevantes

---

**Noticias de Tecnología e IA**
1. [Java4Shell: Vulnerabilidad de ejecución remota de código en OpenJDK por Base64](#item-tech-news-1) ⭐️ 9.0/10
2. [OpenAI lanza los modelos GPT-6.2 Astra y Sol](#item-tech-news-2) ⭐️ 9.0/10
3. [El repositorio de ONNX Runtime de Microsoft desaparece de GitHub](#item-tech-news-3) ⭐️ 8.0/10
4. [Lanzamiento del número 73 de la revista Phrack](#item-tech-news-4) ⭐️ 8.0/10
5. [Patrón de sandboxes externos para aislar código ejecutado por agentes de IA](#item-tech-news-5) ⭐️ 8.0/10
6. [Actualización de llama.cpp b12503 mejora el soporte y rendimiento de OpenVINO](#item-tech-news-6) ⭐️ 7.0/10

**Blogs Técnicos e Ingeniería**
1. [Aceleración de la decodificación en vLLM con FlyDSL MonoKernels](#item-tech-blog-1) ⭐️ 8.0/10

---

## Noticias de Tecnología e IA

<a id="item-tech-news-1"></a>
### [Java4Shell: Vulnerabilidad de ejecución remota de código en OpenJDK por Base64](https://calif.io/java4shell/) ⭐️ 9.0/10

Investigadores han analizado y demostrado una vulnerabilidad crítica de ejecución remota de código \(RCE\) en OpenJDK, denominada Java4Shell, que afecta al procesamiento de Base64. La explotación requiere condiciones específicas y depende de la máquina virtual utilizada, como HotSpot, mientras que otras como OpenJ9 no se ven afectadas. El ataque aprovecha técnicas complejas de manipulación de memoria y se ve influenciado por las condiciones de la red, como la latencia y la fluctuación.

hackernews · werrett · Nov 17, 21:11 · [Discusión](https://news.ycombinator.com/item?id=50538240)

**「Antecedentes」** El 17 de noviembre de 2026 se divulgó públicamente Java4Shell \(CVE-2026-114938\), una vulnerabilidad crítica de corrupción de memoria en el decodificador Base64 de OpenJDK descubierta por investigadores de seguridad de Calif.

**「Impacto」** Muchos hosts que ejecutan compilaciones de OpenJDK, Oracle JDK o GraalVM quedan expuestos a posibles ataques si cumplen las condiciones específicas de vulnerabilidad, lo que ha llevado a organizaciones a publicar scripts de detección para mitigar el riesgo.

**「Discusión de la comunidad」** Los comentaristas destacaron la complejidad técnica de la explotación y la necesidad de condiciones de red estables, mientras que algunos compartieron scripts de detección gratuitos para identificar las configuraciones de VM vulnerables. También se sugirió de forma no confirmada que el fallo podría estar ligado a la implementación de AVX512 para la decodificación de Base64.

<details><summary>Referencias</summary>
<ul>
<li><a href="https://www.sophos.com/en-us/security-advisories/sophos-sa-20261118-java4shell">Advisory: OpenJDK Base64 Vulnerability - Java4Shell (CVE-2026 ...</a></li>
<li><a href="https://semgrep.dev/blog/2026/java4shell-openjdk-base64-vulnerability/">Java4Shell: Critical OpenJDK Base64 RCE (CVE-2026-114938)</a></li>

</ul>
</details>

**Etiquetas**: `#java`, `#security`, `#vulnerability`, `#openjdk`, `#rce`

---

<a id="item-tech-news-2"></a>
### [OpenAI lanza los modelos GPT-6.2 Astra y Sol](https://openai.com/index/introducing-gpt-6-2-astra-sol) ⭐️ 9.0/10

OpenAI ha lanzado GPT-6.2 Astra y GPT-6.2 Sol en la API como \`gpt-6.2-astra\` y \`gpt-6.2-sol\`, mejorando el rendimiento en codificación y uso de ordenador. GPT-6.2 Astra tiene un precio de entrada de $8 por millón de tokens y $40 por millón de tokens de salida, mientras que el precio con caché se reduce a $0.40 por millón. GPT-6.2 Sol mantiene el coste de $2 por millón de tokens de entrada y $10 por millón de tokens de salida.

rss · OpenAI News · Nov 17, 17:45

**「Contexto de modelos y precios de OpenAI」** Estos modelos continúan la línea de versiones anteriores de la familia Astra y Sol de OpenAI, que ofrecen diferentes equilibrios entre coste, eficiencia y capacidad para tareas complejas o cotidianas.

**「Impacto en costes para sesiones de agentes」** La reducción en el precio de los tokens con caché en GPT-6.2 Astra beneficia de manera directa las ejecuciones prolongadas de sesiones de agentes, abaratando su coste operativo.

**Etiquetas**: `#artificial intelligence`, `#machine learning`, `#language models`, `#software engineering`, `#industry news`

---

<a id="item-tech-news-3"></a>
### [El repositorio de ONNX Runtime de Microsoft desaparece de GitHub](https://github.com/microsoft/onnxruntime) ⭐️ 8.0/10

El repositorio oficial de ONNX Runtime de Microsoft en GitHub ha dejado de estar accesible de manera repentina. Esta desaparición se produce en paralelo a discusiones en la comunidad sobre posibles incidentes de seguridad en la cadena de suministro y preocupaciones en torno a la telemetría integrada. Hasta el momento no se han publicado los motivos oficiales de la retirada ni se ha confirmado la relación con incidentes concretos.

hackernews · nvader · Nov 17, 23:18 · [Discusión](https://news.ycombinator.com/item?id=50539610)

**「Antecedentes」** ONNX Runtime es un motor de inferencia de código abierto ampliamente utilizado para desplegar modelos de aprendizaje automático y de inteligencia artificial en diversos entornos de producción.

**「Discusión de la comunidad」** Los usuarios señalaron que ONNX incluye mecanismos de telemetría sin opciones sencillas para desactivarlos, y relacionaron la caída del repositorio con problemas recientes de seguridad en otros paquetes de Microsoft y con debates sobre vulnerabilidades en la cadena de suministro de IA.

**Etiquetas**: `#artificial intelligence`, `#open source`, `#security`, `#github`, `#machine learning`

---

<a id="item-tech-news-4"></a>
### [Lanzamiento del número 73 de la revista Phrack](https://phrack.org/issues/73/introduction_md) ⭐️ 8.0/10

La revista de seguridad informática Phrack ha publicado su número 73, el cual incluye artículos técnicos y de investigación sobre vulnerabilidades como los escapes de contenedores. Esta nueva edición continúa con la larga tradición de publicación de material técnico avanzado en la comunidad de hackers.

hackernews · notmine1337 · Nov 17, 18:31 · [Discusión](https://news.ycombinator.com/item?id=50535992)

**「Antecedentes」** Phrack es una de las publicaciones periódicas sobre seguridad informática y hacking más antiguas y reconocidas, fundada originalmente en la década de 1980.

**「Discusión en la comunidad」** Los lectores comentaron sobre la evolución de la revista desde sus inicios en los años 90 y debatieron sobre aspectos como la divulgación responsable de los exploits publicados y la nostalgia por el formato tradicional y abierto de estos fanzines.

**Etiquetas**: `#security`, `#exploit`, `#open source`, `#computer systems`

---

<a id="item-tech-news-5"></a>
### [Patrón de sandboxes externos para aislar código ejecutado por agentes de IA](https://simonwillison.net/2026/Nov/17/external-sandboxes-for-coding-agents/) ⭐️ 8.0/10

Simon Willison y el laboratorio de investigación Prime Radiant han presentado el patrón de &quot;sandbox externo&quot; para aislar de forma segura el código ejecutado por agentes de inteligencia artificial de la máquina host. Para demostrar esta arquitectura, han publicado tres implementaciones de servidores sandbox con una API de localhost idéntica: \`external-sandbox-v86\` \(que utiliza Alpine Linux en WebAssembly mediante v86\), \`external-sandbox-container\` \(que emplea Apple Containers\) y \`external-sandbox-quicksand\` \(basado en la biblioteca Quicksand de Microsoft\). Las soluciones se pueden configurar con herramientas como Pi, Claude Code o Codex, e incluyen un proxy opcional con lista blanca de HTTP/HTTPS y un mecanismo de reemplazo de credenciales para realizar llamadas autenticadas sin exponer secretos.

rss · Simon Willison · Nov 17, 22:52

**「Antecedentes」** La ejecución de código generado por modelos de lenguaje plantea riesgos significativos de seguridad, tales como ataques de inyección de instrucciones o la realización accidental de acciones destructivas en el sistema de archivos local.

**「Impacto」** Los desarrolladores e ingenieros que prueben agentes de código locales o modelos experimentales pueden utilizar estas implementaciones para mitigar el riesgo de ejecución de comandos maliciosos y restringir estrictamente las comunicaciones de red del agente.

**Etiquetas**: `#artificial intelligence`, `#software engineering`, `#security`, `#coding agents`, `#sandboxing`

---

<a id="item-tech-news-6"></a>
### [Actualización de llama.cpp b12503 mejora el soporte y rendimiento de OpenVINO](https://github.com/ggml-org/llama.cpp/releases/tag/b12503) ⭐️ 7.0/10

La versión b12503 de llama.cpp actualiza el backend de OpenVINO para optimizar el uso de memoria y corregir la detección de máscaras de Atención de Ventana Deslizante \(SWA\) junto con los índices de la caché KV. Los cambios incluyen la derivación de tamaños de atención directamente a partir de la forma de la máscara KQ, la habilitación de un caché KV apátrida de 4 dimensiones para la GPU, y mejoras en la atención agrupada por consultas \(GQA\) para permitir la fusión en el núcleo SDPA. Adicionalmente, se introdujo una caída automática a ejecución apátrida al desactivar la atención flash \(-fa off\).

github · github-actions\[bot\] · Nov 18, 08:28

**「Contexto técnico」** El backend OpenVINO en llama.cpp permite ejecutar modelos de lenguaje grande \(LLM\) de forma eficiente utilizando hardware de Intel, como procesadores, gráficos integrados y unidades de procesamiento neuronal \(NPU\). Las optimizaciones previas en la gestión de cachés y la fusión de operaciones de atención son fundamentales para reducir la sobrecarga de memoria durante la generación de tokens.

**「Impacto operativo」** Los usuarios que ejecutan modelos con hardware compatible mediante OpenVINO experimentarán una reducción en las asignaciones repetidas de memoria y un mejor rendimiento en la fusión de kernels de atención, particularmente al procesar capas con ventanas deslizantes o configuraciones de atención agrupada.

**Etiquetas**: `#Machine Learning`, `#LLM Inference`, `#OpenVINO`, `#Open Source`, `#Artificial Intelligence`

---

## Blogs Técnicos e Ingeniería

<a id="item-tech-blog-1"></a>
### [Aceleración de la decodificación en vLLM con FlyDSL MonoKernels](https://vllm.ai/blog/2026-11-18-flydsl-monokernels) ⭐️ 8.0/10

rss · vLLM Blog · Nov 18, 00:00

**「Antecedentes」** En las aplicaciones interactivas de modelos de lenguaje, la fase de decodificación a baja concurrencia sufre una gran sobrecarga debido al lanzamiento constante de múltiples y pequeños núcleos en la GPU que realizan poco trabajo efectivo de forma aislada.

**「Solución」** Los autores detallan cómo los MonoKernels escritos en FlyDSL combinan etapas dependientes de operadores en lanzamientos persistentes de GPU en hardware AMD Instinct, reutilizando bloques de hilos y adelantando la carga de pesos para solapar el tráfico de memoria. Esta técnica reduce drásticamente los tiempos muertos entre operaciones y se integra de forma transparente en vLLM mediante un enfoque opcional por capas, manteniendo la precisión numérica intacta en múltiples modelos evaluados.

**「Conclusión」** La adopción de FlyDSL MonoKernels demuestra que eliminar las fronteras innecesarias entre núcleos mejora notablemente la interactividad en escenarios de baja concurrencia para la inferencia de LLMs.

**Etiquetas**: `#GPU Optimization`, `#vLLM`, `#LLM Inference`, `#Compilers and DSLs`, `#AMD ROCm`

---