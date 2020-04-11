# prueba2
<!DOCTYPE html>
<html lang="es">
<head>
	<title>OVI - Diseño Web </title>

	<meta charset="UTF-8">
	
	<!-- Etiquetas SEO -->
	<meta content="Diana Carolina Talero" name="author">
	<meta content="Describir los elementos básicos para el diseño web" name="description">
	<meta content="GIT, HTML, CSS, UNAD" name="keywords">
	
	<!-- Etiqueta visualización viewport -->
	<meta name="viewport" content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0">

	<!-- Estilos -->
		<style type="text/css">
		*{
			margin:0;
			padding:0;
			font-family:Arial;
			box-sizing: border-box;
		}

		main{
			width:100%;
		}

		#header{
			top:0;
			left:0;
			margin:auto;
			width:100%;
			min-width: 1024px;
			height:100px;
			position:fixed;
			z-index:1000;
			background-color:rgba(255,255,255,1);
			-webkit-box-shadow: 3px 10px 13px -6px rgba(0,0,0,0.45);
			-moz-box-shadow: 3px 10px 13px -6px rgba(0,0,0,0.45);
			box-shadow: 3px 10px 13px -6px rgba(0,0,0,0.45);
		}

		.subheader{
			width:90%;
			margin:5px auto;
			border-collapse: separate;
		}

		.col1{
			width:300px;
			text-align: center;
		}

		.col2{
			width:90%;
			margin:auto;
			padding-left:12px;
		}

		.logo{
			width:250px;
			height:auto;
			padding:10px;
		}

		ul, li{
			text-align:center;
			list-style: none;
		}

		#nav {
			list-style:none inside;
			margin:0;
			padding:0;
			text-align:center;
			}

		#nav li {
			display:block;
			position:relative;
			float:left;
			background: #144277; /* menu background color */
			}

		#nav li a {
			display:block;
			padding:0;
			text-decoration:none;
			width:200px; /* this is the width of the menu items */
			line-height:35px; /* this is the hieght of the menu items */
			color:#ffffff; /* list item font color */
			}
				
		#nav li li a {font-size:80%;} /* smaller font size for sub menu items */
			
		#nav li:hover {background:#145277;} /* highlights current hovered list item and the parent list items when hovering over sub menues */



		/*--- Sublist Styles ---*/
		#nav ul {
			position:absolute;
			padding:0;
			left:0;
			display:none; /* hides sublists */
			}

		#nav li:hover ul ul {display:none;} /* hides sub-sublists */

		#nav li:hover ul {display:block;} /* shows sublist on hover */

		#nav li li:hover ul {
			display:block; /* shows sub-sublist on hover */
			margin-left:200px; /* this should be the same width as the parent list item */
			margin-top:-35px; /* aligns top of sub menu with top of list item */
			}

		#inicio{
			width:100%;
			height:80vh;
			position:relative;
			background-image:url('img/cursovirtual.jpg');
			background-repeat:no-repeat;
			background-attachment: fixed;
			background-size:100%;
			background-origin: content-box;
			background-position: top center;
		}
		.row{
			width:90%;
			margin:auto;
		}
		.info{
			width:90%;
			margin:auto;
			border-collapse: separate;
			border-spacing:5px;
		}
		.side{
			width:35%;
			height:450px;
			padding:10px;
			border-radius:7px;
			background-color:rgba(255,218,0,1);
		}
		.side tr{
			border-radius:7px;
			background-color:rgba(255,255,255,1);
		}
		.side td{
			padding:10px;
		}
		td p{
			text-align: justify;
		}
		td>li{
			list-style-type: square;
			text-align:justify;
		}
		h2{
			width:100%;
			color:#BC3808;
			line-height: 4rem;
			border-radius:7px;
			text-align: center;
			background-color:rgba(255,218,0,1);
		}
		#tematica{
			width:100%;
			padding:20px;
			vertical-align: center;
			background-color:rgba(255,255,255,1);
		}
		.row h1{
			padding:10px;
			margin:auto;
			font-size:42px;
			text-align: center;
			color:rgba(255,255,255,1);
			background-color:rgba(51,51,51,1);
		}
		.fila{
			width:100%;
			margin:auto 180px;
			margin:auto 180px;
			display:inline-flex;
		}
		figure:nth-child(1){
			padding:0;
		}
		figure{
			padding-left:25px;
		}
		#titulo1{
			width:364px;
			height:70px;
			overflow:hidden;
			vertical-align: middle;
			background-color:rgba(165,70,134,1);
		}
		#titulo1>h3{
			padding:15px;
			text-align: center;
			color:rgba(255,255,255,1);
			text-shadow: rgb(46, 46, 46) 0px 4px 5px;
		}
		#titulo2{
			width:364px;
			height:70px;
			overflow:hidden;
			vertical-align: middle;
			background-color:rgba(244,121,32,1);
		}
		#titulo2>h3{
			padding:15px;
			text-align: center;
			color:rgba(255,255,255,1);
			text-shadow: rgb(46, 46, 46) 0px 4px 5px;
		}
		#titulo3{
			width:364px;
			height:70px;
			overflow:hidden;
			text-align:center;
			background-color:rgba(80,183,72,1);
		}
		#titulo3>h3{
			padding:15px;
			text-align: center;
			color:rgba(255,255,255,1);
			text-shadow: rgb(46, 46, 46) 0px 4px 5px;
		}
		#titulo4{
			width:364px;
			height:50px;
			overflow:hidden;
			vertical-align: middle;
			background-color:rgba(240,180,41,1);
		}
		#titulo4>h3{
			padding:15px;
			text-align: center;
			color:rgba(255,255,255,1);
			text-shadow: rgb(46, 46, 46) 0px 4px 5px;
		}
		#titulo5{
			width:364px;
			height:50px;
			overflow:hidden;
			vertical-align: middle;
			background-color:rgba(67,99,244,1);
		}
		#titulo5>h3{
			padding:15px;
			text-align: center;
			color:rgba(255,255,255,1);
			text-shadow: rgb(46, 46, 46) 0px 4px 5px;
		}
		figcaption{
			width:364px;
			text-align:center;
			background-color:rgba(179,179,179,.3);
		}
		figcaption>p{
			padding:10px;
		}
		#informes{
			width:100%;
			height:70vh;
			background-image:url('img/agent-18762_1280.jpg');
			background-repeat:no-repeat;
			background-attachment: fixed;
			background-size:35% 100%;
			background-position: left;
		}
		.datos{
			width:70%;
			margin:auto;
			padding-top:130px;
			padding-left:300px;
			border-collapse: separate;
			border-spacing: 5px;
			text-align: center;
		}
		.datos>strong{
			text-align: center;
		}
		.contacto{
			color:rgba(0,102,128,1) !important;
			background-color:transparent !important;
		}

		footer{
			width:100%;
			max-height:20%;
			vertical-align: middle;
			background-color:rgba(0,88,131,1);
		}
		.aside{
			width: 48%;
			margin:30px auto;
			border-color:yellow solid 2px;
			display:inline-block;
		}
		.aside a{
			color:rgba(255,255,255,1);
			text-decoration: none;
		}
		.block{
			width:100%;
			border-spacing: 5px;
			border-collapse: separate;
			color:rgba(255,255,255,1);
		}
		#counter{
			color:rgba(253,245,0,1);
			text-align:center;
			font-size: 38px;
			font-weight: 700;
		}

		.linkq:hover{
			zoom:1.1;
			cursor:pointer;
		}
	</style>
	
	<script type="text/javascript" src="js/jquery-3.1.1.min.js"></script>
<body>

	<!-- Contenedor principal -->
	<main>
		<div id="header"> <!-- Contenedor del menú -->
			<table class="subheader">
				<tr>
					<td class="col1">
						<a href="https://www.unad.edu.co"><img src="img/unad.png" class="logo" alt="Universidad Nacional Abierta y a Distancia"></a>
					</td>
					<td class="col2">
						<ul id="nav">
						  <li><a href="index.html">Inicio</a></li>
						  <li><a>Lecturas</a>
							<ul>
							  <li><a>GIT/GITHUB &raquo;</a>
								<ul>
								  <li><a href="lectura1.html#lectura1">CVS</a></li>
								  <li><a href="lectura1.html#lectura2">GIT</a></li>
								  <li><a href="lectura1.html#lectura3">GITHUB</a></li>
								</ul>
							  </li>
							  <li><a>HTML &raquo;</a>
								<ul>
								  <li><a href="lectura2.html#lectura1">¿Que es?</a></li>
								  <li><a href="lectura2.html#lectura2">HTML5</a></li>
								  <li><a href="lectura2.html#lectura2">Ventajas</a></li>
								</ul>
							  </li>
							  <li><a>CSS&raquo;</a>
								<ul>
								  <li><a href="lectura3.html#lectura1">¿Que es?</a></li>
								  <li><a href="lectura3.html#lectura2">Ventajas</a></li>
								</ul>
							  </li>								  
							</ul>
						  </li>
						  <li><a href="multimedia.html#multimedia">Multimedia </a>
							<ul>
							<li><a href="multimedia.html#video1">GIT/GITHUB</a></li>
							<li><a href="multimedia.html#video2">HTML</a></li>
							<li><a href="multimedia.html#video3">CSS</a></li>									
							</ul>
						  </li>
						  <li><a href="autor.html">Autor </a></li>
						  <li><a>Actividades </a>
							<ul>
							<li><a href="actividad1.html">Actividad 1</a></li>
							<li><a href="actividad2.html">Actividad 2</a></li>									
							</ul>
						  </li>						  
						</ul>
					</td>
				</tr>
			</table>
		</div>

		<!-- Banner inicial -->
		<section id="inicio"></section>

		<!-- Sección que contiene la información general del curso -->
		<section id="info">
			<div class="container">
			<br>
			<br>
			<h2>
			Estimado (a)  visitante, bienvenido al Objeto Virtual de Información O.V.I. sobre los elementos básicos en el diseño web tales como la gestión de proyectos colaborativos y los lenguajes HTML5 y CSS3, diseñado por Diana Carolina Talero. En este material encontrará contenidos de lectura y contenidos multimedia que le ayudaran en el desarrollo de las actividades académicas relacionadas con el tema.
			</h2>
			</div>
			<br>
			<br>
			<div class="container">
				<div class="row" style="padding-top:40px; padding-bottom:40px;">
					<table class="info">
						<tr>
							<td><h2>Información General</h2></td>

							<td></td>

							<td><h2>Objetivos</h2></td>
						</tr>

						<tr>
							<td style="width:45%;">
								<table class="side" cellpadding="10" style="width:100%; background-color:rgba(255,218,0,1);">
									<tr>
										<td><strong>Código:</strong></td>
										<td>301122</td>
									</tr>

									<tr>
										<td><strong>Curso:</strong></td>
										<td>Diseño de Sitios Web</td>
									</tr>

									<tr>
										<td><strong>Programa:</strong></td>
										<td>Ingeniería de Sistemas </td>
									</tr>

									<tr>
										<td><strong>Temática:</strong></td>
										<td>GIT/GITHUB, HTML5 y CSS3</td>
									</tr>

									<tr>
										<td><strong>Descripción:</strong></td>
										<td>
											<p>Introducción, profundización e información complementaria sobre el uso de GIT y GITHUB para gestionar proyectos colaborativos de diseño web, HTML5 y CSS3 para creación  de contenidos en formato web (Paginas y Sitios Web)</p>
										</td>
									</tr>
								</table>
							</td>

							<td style="width:10%;"></td>

							<td style="width:45%;">
								<table class="side" style="width:100%; background-color:rgba(255,218,0,1);">
									<tr>
										<td>
											<li>Describir los elementos básicos para el diseño web</li>
										</td>
									</tr>

									<tr>
										<td>
											<li>Explicar el uso básico de GIT y GITHUB en la gestión de proyectos de diseño web</li>
										</td>
									</tr>

									<tr>
										<td>
											<li>Mostrar los elementos básicos del lenguaje HTML5 como herramienta para estructurar y presentar el contenido para la web</li>
										</td>
									</tr>

									<tr>
										<td>
											<li>Mostrar las propiedades básicas del lenguaje CSS3 para definir la presentación de un documento estructurado escrito en HTML5</li>
										</td>
									</tr>
								</table>
							</td>
						</tr>
					</table>
				</div>
			</div>
		</section>

		
		<section id="tematica">
			<div class="container">
				<div class="row">
					<h1>¿Que encontraras en este O.V.I?</h1>
					<br>
				</div>
				
				<br>

				<div class="fila" id="contenedor">
					<figure>
						<div id="titulo1"><h3> GIT y GITHUB</h3></div>
						<img src="img/github.png" alt="diagramando" width="364" height="288">
						<figcaption><p>Dar una breve introducción a la gestión de proyectos colaborativos alojados en GITHUB mediante el manejo de versiones con GIT. </p></figcaption>
					</figure>


					<figure>
						<div id="titulo2"><h3>HTML5 - Estructura y contenido de una página Web</h3></div>
						<img src="img/html5.png" alt="diagramando" width="364" height="288">
						<figcaption><p>Mostrar los elementos básicos del lenguaje estructurado HTML5 .</p></figcaption>
					</figure>
					
					
					<figure>
						<div id="titulo3"><h3>CSS3 - Estilo de una pagina web</h3></div>
						<img src="img/css.png" alt="diagramando" width="364" height="288">
						<figcaption><p>Mostrar los elementos básicos del lenguaje CSS3 para la presentación del documento HTML5 .</p></figcaption>
					</figure>
				</div>

				<br><br><br>
			</div>
		</section>

		<!-- Pie de página -->
		<footer>
			<div class="container">
				<div class="row">
					<div class="aside">
						<table class="block">
							<tr>
								<td colspan="2">
									<small>Diseño y Creación: <a href="autor.html">Diana Carolina Talero</a> &#174;</small>
									<br>
								<td>
							</tr>
							<tr>
								<td>
									<img src="img/commons.png" alt="license" style="width:100px; height:auto;">
									<br>
								</td>
							</tr>

							<tr>
								<td>Eres el visitante No.</td>
							</tr>
							
							<tr>
								<td>
							<!-- Contador de visitas -->
							<center><a href="http://www.websmultimedia.com/contador-de-visitas-gratis" title="Contador De Visitas Gratis">
							<img style="border: 0px solid; display: inline;" alt="contador de visitas" src="http://www.websmultimedia.com/contador-de-visitas.php?id=260897"></a><br><a href='http://www.websmultimedia.com/contador-de-visitas-gratis'></a><br><a href='http://www.websmultimedia.com'></a></center>
							<!-- Fin Contador de visitas -->
								</td>
							</tr>

							<tr>
								<td><img src="img/sellos_calidad.png" alt="Calidad" style="width:65%; height:auto;"></td>
							</tr>
						</table>
					</div>

					<div class="aside">
						<a class="twitter-timeline" data-height="400" href="https://twitter.com/UniversidadUNAD?ref_src=twsrc%5Etfw">Tweets by Universidad UNAD</a> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>					</div>
					</div>
				</div>
			</div>
		</footer>
	</main>
	
	<script type="text/javascript" src="js/jquery-3.1.1.min.js"></script>
	<script type="text/javascript">
		//Hacemos la Function para abrir el contador de visitas
		function recargar_views(){
			$(".views").load("contador.txt");
		}

		// Establecemos el temporizador a 1 segundos
		timer = setInterval("recargar_views()", 1000);
	</script>
	
</body>
</html>
