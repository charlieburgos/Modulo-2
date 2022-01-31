<!DOCTYPE html>
<html>
<head>
    <meta charset= "UTF-8">
    <title>Formulario de Contacto</title>
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<link rel="stylesheet" href="form.css">
    <!-- Bootstrap CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet"
        integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" crossorigin="anonymous" />
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.7.2/font/bootstrap-icons.css" />
    <style>
    .abs-center {
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 100vh;
  }
  
  .form {
    width: 450px;
  }
    </style>

</head>
<body>
<!-- Inicio Formulario -->
<div class="container">
	<div class="abs-center">
		<form class="row g-3 needs-validation form" novalidate method="get" action="" id="form">
			<fieldset>
				<legend>Formulario de Contacto</legend>
				<div class="form-group">
					<div class="row">
						<div class="col">
							<label for="nombre">Nombre</label>
							<input class=form-control type="text" name="nombre" id="nombre" pattern="{2,48}" required placeholder="INGRESE NOMBRE"/>
							<i class="fa fa-check check-ok"></i>
						</div>
					</div>
				</div>
				<div class="form-group">
					<div class="row">
						<div class="col">
							<label for="apellido_paterno">Apellido Paterno</label>
							<input class=form-control type="text" name="apellidop" id="apellidop" pattern="{2,64}" required placeholder="INGRESE APELLIDO"/>
							<i class="fa fa-check check-ok"></i>
						</div>
						<div class="col">
							<label for="apellido_materno">Apellido Materno</label>
							<input class=form-control type="text" name="apellidom" id="apellidom" pattern="{2,64}" required placeholder="INGRESE APELLIDO"/>
							<i class="fa fa-check check-ok"></i>
						</div>
					</div>
				</div>
				<div class="form-group">
					<div class="row">
						<div class="col" >
							<label for="correo">Email</label>
							<input class=form-control type="email" name="correo" id="correo" required placeholder="INGRESE EMAIL"/>
							<i class="fa fa-check check-ok"></i>
						</div>
					</div>
				</div>
				<div class="form-group">
					<div class="row">
						<div class="col">
							<label for="domicilio">Domicilio</label>
							<input class=form-control type="text" name="domicilio" id="domicilio" pattern="" required placeholder="ingrese su direccion"/>
							<i class="fa fa-check check-ok"></i>
						</div>
					</div>
					<div class="row">
						<div class="col">
							<label for="edad">Edad</label>
							<input class=form-control  type="number" name="age" id="age" pattern="{8,12}" required placeholder="edad"/>
							<i class="fa fa-check check-ok"></i>
						</div>
					</div>
				</div>	
				<div class="form-group">
					<label	for="alergico">Es Alergico?</label>
					<div class="col form-check">
						<input class="form-check-input" type="radio" name="alergia" id="alergiaSi" value="si" checked>
  						<label class="form-check-label" for="alergiaSi">Si</label>
					</div>
					<div class="col form-check">
						<input class="form-check-input" type="radio" name="alergia" id="alergiasNo" value="no" checked>
  						<label class="form-check-label" for="alergiasNo">No</label>
					</div>
				</div>
				<div class="form-group">
					<label for="comentarios">Medicamentos Contraindicados</label>
					<textarea class="form-control" id="comentarios" rows="3"></textarea>
				</div>
				<div>
				<button class= "btn btn-primary" type="submit">Enviar</button>
				</div>
			</fieldset>
		</form>
	</div>
</body>
</html>
