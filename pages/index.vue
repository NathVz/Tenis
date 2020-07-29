<template>
<div>
    <!-- ======= Banner Principal Section ======= -->
    <section id="topbar" class="d-none d-lg-block">
        <div class="container">
            <img src="~assets/img/logo-tennis.png" alt="" width="37">
        </div>
    </section>
    <hr class="vr">
	<div class="menu">
		<b-nav>
			<b-nav-item active>Inicio</b-nav-item>
			<b-nav-item>Acerca de nosotros</b-nav-item>
			<b-nav-item>Historia</b-nav-item>
			<b-nav-item>Contacto</b-nav-item>
		</b-nav>
	</div>

    <section id="hero" class="d-flex align-items-center">
        <div class="container">
			<div class="ctn-banner">
				<h1>Las mejores raquetas para <br> jugar <span>Tennis</span></h1>
				<div class="mt-5 mt-lg-5 text-lg-left">
					<a class="btn-acerca" href="#"> Acerca de nosotros
						<svg xmlns="http://www.w3.org/2000/svg" width="23" height="6" viewBox="0 0 23 6">
						<path fill="#fff" fill-rule="evenodd" d="M22.908 2.7L20.428.128a.39.39 0 0 0-.579 0 .425.425 0 0 0 0 .6l1.778 1.843H.413C.165 2.57 0 2.74 0 3c0 .257.165.428.413.428h21.213l-1.779 1.844a.425.425 0 0 0 0 .6.44.44 0 0 0 .29.128.44.44 0 0 0 .289-.129l2.48-2.572a.531.531 0 0 0 .002-.6z"/>
						</svg>
					</a>
				</div>
			</div>
        </div>
    </section>
  <!-- ======= Raqueta.Accesorios Section ======= -->
    <section id="conoce" class="d-flex align-items-center">
        <div class="container">
            <div class="row text-center text-md-left">
                <div class="col-sm-12 col-md-3 col-lg-3 tennis text-center text-lg-right">
                    <p>TENNIS</p>
                </div>
                <div class="col-sm-12 col-md-5 col-lg-6 conoceText">
                    <h2>Raquetas.Accesorios.<br>Pelotas.</h2>
                    <p>Conoce nuestras raquetas y aprende a jugar <br>
                    Tennis cómo un profesional.</p>
                </div>
                <div class="col-sm-12 col-md-4 col-lg-3 mt-3 mt-lg-0 ctn-btnH">
                    <a class="btn-historia" href="#"> Historia 
						<svg xmlns="http://www.w3.org/2000/svg" width="23" height="6" viewBox="0 0 23 6">
 						<path fill="#29304A" fill-rule="evenodd" d="M22.908 2.7L20.428.128a.39.39 0 0 0-.579 0 .425.425 0 0 0 0 .6l1.778 1.843H.413C.165 2.57 0 2.74 0 3c0 .257.165.428.413.428h21.213l-1.779 1.844a.425.425 0 0 0 0 .6.44.44 0 0 0 .29.128.44.44 0 0 0 .289-.129l2.48-2.572a.531.531 0 0 0 .002-.6z"/>
						</svg>
					</a>
                </div>
            </div>
        </div>
    </section>

  <!-- ======= Nuestras Raquetas Section ======= -->
    <section id="raquetas" class="">
        <div class="container-fluid">
            <div class="row">
                <div class="col-12 col-md-12 col-lg-4 col-xl-4 bg-ball">
                    <div class="ctn-ball">
                        <div class="ctn-title text-center text-md-left text-lg-left">
                            <h2>Nuestras<br><span>Raquetas</span> </h2>
                            <p>Conoce nuestras raquetas y <br> aprende a jugar Tennis cómo <br>un profesional.</p>
                        </div>
                        <div class="dots-carrusel d-flex justify-content-center justify-content-md-start">
                            <button  class="owl-dot active"><span></span></button>
                            <button  class="owl-dot"><span></span></button>
                            <button  class="owl-dot"><span></span></button>
                            <button  class="owl-dot"><span></span></button>
                        </div>
                        <div class="nav-carrusel mt-4 d-flex justify-content-center justify-content-md-start">
                            <button type="button" role="presentation" id="my-previous-btn" class="owl-prev"><span><i class="fas fa-caret-left"></i></span></button>
                            <button type="button" role="presentation" id="my-next-btn" class="owl-next"><span><i class="fas fa-caret-right"></i></span></button>
                        </div>
                    </div>
                </div>
                <div class="col-12 col-md-12 col-lg-8 col-xl-8 ctn-div">
                    <div class="ctn-carrusel">
						<carousel :autoplay="true" :nav="false" :responsive="{0:{items:1,nav:false},600:{items:2,nav:false},760:{items:3,nav:false},900:{items:3,nav:false}}">
							<img src="~assets/img/products/raqueta1.png" alt="">
							<img src="~assets/img/products/raqueta2.png" alt="">
							<img src="~assets/img/products/raqueta3.png" alt="">
							<img src="~assets/img/products/raqueta4.png" alt="">
						</carousel>
                    </div>
                </div>
            </div>
        </div>
    </section>

<!-- ======= Banner Cancha Section ======= -->
    <section id="banner-cancha">
        <div class="container">
        </div>
    </section>
</div>

</template>

<script lang="js">
import Vue from 'vue'
import carousel from 'vue-owl-carousel'

export default Vue.extend({
    components: { carousel },
})

</script>

<style lang="scss">
@import '~assets/css/main.scss';

#topbar{
    position: absolute;
    top: 25px;
    left: 36px;
}
.vr{
    border: none;
    border-left: 1.2px solid  $white;
    width: 1px; 
    position: absolute;
    top: -18px;   
	z-index: 0;
	@include for-phone{
		left: 30px;
		height: 80vh;
	}
	@include for-tablet{
		left: 50px;
		height: 100vh;
	}
	@include for-desktop{
		left: 125px;
		height: 100vh;
	}
}
.menu {
	position: absolute;
	left: 180px;
	top: 7%;
	a.nav-link {
	color:  $white;
	font-size: 16px;
    letter-spacing: 1.5px;
	font-family: HelveticaNeue, sans-serif;
		&:hover{
			color: $sickly-yellow;
		}
	}
	@include for-phone{
		display: none;
	}
	@include for-tablet{
		left: 90px;
	}
	@include for-desktop{
		left: 180px;
	}
}
#hero {
	width: 100%;
	background-size: cover;
	background-image: url("~assets/img/banner.jpg");
	@include for-phone{
		height: 80vh;
	}
	@include for-tablet{
		height: 100vh;
	}
	@include for-desktop{
		height: 100vh;
	}
	.ctn-banner{
		position: absolute;
        left: 180px;
		top: 280px;
		@include for-phone{
			left: 60px;
			top: 160px;
		}
		@include for-tablet{
			left: 90px;
			top: 240px;
		}
		@include for-desktop{
			left: 180px;
			top: 280px;
		}
	}
	h1 {
		font-size: 53px;
		line-height: 68px;
		line-height: 1.28;
		letter-spacing: -0.05px;
		color: $white;
		@include for-phone{
		font-size: 43px;
		}
		span {
			color: $sickly-yellow;
			font-weight: 700;
		}
	}
	.btn-acerca {
		font-family: HelveticaNeue, sans-serif;
		font-size: 13px;
		padding: 15px 30px;
		letter-spacing: 1px;
		width: 269px;
		height: 53px;
		font-weight: 500;
		border-radius: 26.5px;
		color: $white;
		border: 1.2px solid $white;
		text-decoration: none;
		position: relative;
		text-transform: uppercase;
		&:hover{
			color: $sickly-yellow;
			border: 1.2px solid $sickly-yellow;	
		}
	}
}
#conoce {
	width: 100%;
	height: 392px;
	background-color: #f3f4f8;
	.tennis {
		p {
			font-size: 15px;
			font-weight: 500;
			margin-top: 12px;
			font-stretch: normal;
			font-style: normal;
			line-height: 2;
			letter-spacing: 1.87px;
			color: $sickly-yellow;
		}
	}
	.conoceText {
		h2 {
			font-size: 50px;
			font-weight: normal;
			font-stretch: normal;
			font-style: normal;
			line-height: 1.14;
			letter-spacing: -0.06px;
			color: #1e2335;
			@include for-phone{
				font-size: 30px;
			}
		}
		p {
			font-size: 18px;
			font-weight: normal;
			font-stretch: normal;
			font-style: normal;
			line-height: 1.78;
			letter-spacing: 0.51px;
			color: #787878;
			margin-top: 20px;
			@include for-phone{
				font-size: 12px;
			}
		}
	}
	.btn-historia {
		width: 210px;
		height: 53px;
		border-radius: 26.5px;
		border: solid 1.2px #282e47;
		font-family: HelveticaNeue, sans-serif;
		font-size: 13px;
		font-weight: 600;
		padding: 15px 30px;
		line-height: 2.15;
		letter-spacing: 1.01px;
		color: #273048;
		text-decoration: none;
		text-transform: uppercase;
		margin-left: 40px;
		&:hover{
			color: $sickly-yellow;
			border: 1.2px solid $sickly-yellow;	
		}
		@include for-phone{
			margin-left: 0px;
		}
		@include for-tablet{
			margin-left: 0px;
		}
	}
	.ctn-btnH{
		@include for-phone{
		display: flex;
        align-items: center;
        justify-content: center;
		}
		@include for-tablet{
		display: flex;
        align-items: center;
        justify-content: center;
		}
		@include for-desktop{
		display: flex;
        align-items: flex-end;
        justify-content: flex-end;
		}
	}
	
}
#raquetas {
	.bg-ball {
		width: 100%;
		height: 468px;
		background-size: cover;
		background-image: url("~assets/img/ball-tennis.png");
	}
	.ctn-title {
		h2 {
			font-size: 50px;
			line-height: 1.28;
			letter-spacing: -0.06px;
			color: $white;
			span {
				font-weight: bold;
			}
		}
		p {
			font-family: HelveticaNeue;
			font-size: 18px;
			line-height: 1.67;
			letter-spacing: 0.51px;
			color: $white;
		}
	}
	.owl-dots {
		display: none;
	}
	.ctn-div{
		display: flex;
		align-items: center;
		width: 100%;
		margin-top: 14px;
        margin-bottom: 14px;
		.ctn-carrusel{
			width: 100%;
			img{
				@include for-phone{
					width:100%
				}
				@include for-tablet{
					width: 90%;
				}
				@include for-desktop{
					width: 90%;
				}
			}
		}
	}
	
	.owl-dot {
		display: inline-block;
		margin: 0 5px;
		width: 5px;
		height: 5px;
		padding: 3px;
		border-radius: 50%;
		background-color: #ebebeb;
		border: 1px solid #ebebeb;
	}
}
.owl-dots {
	margin-top: 5px;
	text-align: center;
}
.ctn-ball {
	margin-top: 60px;
	@include for-tablet{
		float: right;
	}
}


button.owl-dot.active {
	background-color: $sickly-yellow !important;
	border: 1px solid $sickly-yellow !important;
}
button.owl-prev {
	color: #fff;
	border: 1px solid #fff;
	line-height: 1;
	margin-right: 12px;
	border-radius: 50%;
	width: 40px;
	height: 40px;
	background: transparent;
	&:focus{
		outline: none !important;
	}
}
button.owl-next {
	color: #fff;
	border: 1px solid $sickly-yellow;
	box-shadow: 0 3px 2px rgba(0,0,0,.1), 0 3px 3px rgba(0,0,0,.3);
	line-height: 1;
	margin-right: 12px;
	border-radius: 50%;
	width: 40px;
	height: 40px;
	background: $sickly-yellow;
	&:focus{
		outline: none !important;
	}
}

#banner-cancha{
    width: 100%;
    height: 80vh;
    background-size: cover;
    background-image: url("~assets/img/banner_footer.jpg");
}

</style>
