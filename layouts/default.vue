<template>
  <div>
	<header>
		<nav class="navbar navbar-expand-lg navbar-light fixed-top bg-light d-md-none d-lg-none">
			<a class="navbar-brand" href="#"><img src="~assets/img/logo-inverse.png" alt="" width="40"></a>
			<button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
				<span class="navbar-toggler-icon"></span>
			</button>
			<div class="collapse navbar-collapse" id="navbarNav">
				<ul class="navbar-nav">
				<li class="nav-item active">
					<a class="nav-link" href="#">Inicio</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="#">Acerca de nosotros</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="#">Historia</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="#">Contacto</a>
				</li>
				</ul>
			</div>
		</nav>
	</header>
    <Nuxt />
    <!-- ======= Footer ======= -->
    <footer id="footer">
        <div class="container">
            <div class="row d-flex align-items-center">
                <div class="col-lg-6 text-center text-lg-left">
                    <nav class="footer-links text-center text-lg-left  pt-lg-0">
                        <a href="#"><strong>Inicio</strong></a>
                        <a href="#">Acerca de nosotros</a>
                        <a href="#">Historia</a>
                        <a href="#">Contacto</a>
                    </nav>
                    <div class="social-links text-center">
                        <a href="#" class="linkedin"><i class="fab fa-linkedin"></i></a>
                        <a href="#" class="linkedin"><i class="fab fa-vimeo-v"></i></a>
                        <a href="#" class="instagram"><i class="fab fa-instagram"></i></a>
                        <a href="#" class="twitter"><i class="fab fa-twitter"></i></a>
                        <a href="#" class="facebook"><i class="fab fa-facebook-f"></i></a>
                    </div>
                </div>
                <div class="col-lg-6 mt-4 mt-lg-4 text-lg-right text-right">
                    <img src="~assets/img/logo-tennis.png" alt="logotipo-tennis" class="logo-footer">
                </div>
            </div>
        </div>
    </footer>

  </div>
</template>

<script>
export default {
}
</script>

<style lang="scss">
@import '~assets/css/main.scss';

.navbar-toggler {
    color: #fff;
    border-color: unsent !important;
}

#footer {
	background: $sickly-yellow;
	height: 200px;
	padding: 60px 0;
	font-size: 13px;
	font-family: HelveticaNeue, sans-serif;
	@include for-phone{
		font-size: 10px;
	}
	@include for-tablet{
		font-size: 10px;
	}
	.social-links {
		margin-top: 20px;
		display: flex;
		@include for-phone{
		margin-top: 20px;
        display: flex;
        align-items: center;
        justify-content: center;
		}
		@include for-tablet{
		margin-top: 20px;
        display: flex;
        align-items: center;
        justify-content: center;
		}
		@include for-desktop {
		align-items: unset;
        justify-content: unset;
		}
		a {
			font-size: 14px;
			display: flex;
			justify-content: center;
			align-items: center;
			color: #fff;
			border: 1px solid #fff;
			line-height: 1;
			margin-right: 12px;
			border-radius: 50%;
			width: 31px;
			height: 31px;
			text-decoration: none;
			&:hover {
				color: #2b3049;
				border: 1px solid #2b3049;
			}
		}
	}
	.footer-links {
		a {
			color: #2b3049;
			padding-right: 30px;
			letter-spacing: 1.14px;
			text-decoration: none;
			@include for-phone{
				padding-right: 10px;
			}
			@include for-tablet{
				padding-right: 10px;
			}
		}
	}
}
.logo-footer {
	width: 55px;
	@include for-phone{
		width: 35px;
	}
	@include for-tablet{
		width: 35px;
	}
}
</style>
