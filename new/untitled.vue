<!DOCTYPE html>

<head>
	<title> wei hong rong </title>
	<link href="https://fonts.googleapis.com/css?family=IBM+Plex+Sans:300,300i,500,700" rel="stylesheet">
	<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/material-design-iconic-font/2.2.0/css/material-design-iconic-font.min.css">
	<script type="text/javascript" src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
</head>

<body>
	<header>
		<div class='logo'>
			<div>wei - hong - rong</div>
		</div>
		<div>
			<a href=''>resume</a>
			<span class='d'>-</span>
			<a href=''>about/contact</a>
			<span class='d'>-</span>
			<a href=''>instagram</a>
			<span class='d'>-</span>
			<a class='contact'>2019 ©</a>

		</div>
	</header>

	<nav>
		<div>
			<ul class='links'>
				<!---<li><a href=''>A<span>rt</span></a></li>--->
				<li><a href=''>D<span>esign</span></a></li>
				<li><a href=''>P<span>hoto<br>graphy</span></a></li>
				<li><a href=''>+<span>More</span></a></li>
			</ul>
		</div>
	</nav>

	<main>
		<article class='first'>

			<div class='omega'>
	
			</div>

			<div class='alpha'>
				<div></div>
			</div>

			<div class='beta'>
				<div></div>
			</div>

			<div class='gamma'>
				<div></div>
			</div>

			<div class='delta'>
				<div></div>
			</div>

			<div class='epsilon'>
				<div></div>
			</div>

			<div class='zeta'>
				<div></div>
			</div>

			<div class='eta'>
				<div></div>
			</div>

			<div class='iota'>
				<div></div>
			</div>
		</article>
	</main>
</body>

<script type="text/javascript">
var vHeight = $(window).height();
var offset = 3*14 + 50;
var alpha = parseInt(255 * (1/(($('.bottom').offset().top+$('.bottom').height())/(vHeight - offset)))).toString(16);
$('footer').css('backgroundColor','#232323' + alpha);

$(window).bind('resizeEnd',function(){
	vHeight = $(window).height();
});

$('section').scroll(function(){
	var bottom = vHeight - offset;
	var alpha = parseInt(255 * (1/(($('.bottom').offset().top+$('.bottom').height())/(bottom)))).toString(16);
	$('footer').css('backgroundColor','#232323' + alpha);
	$('.animate').each(function() {
		if( $(this).offset().top < bottom){
			$(this).addClass('animated');
			$(this).removeClass('animate');
		}
	});
});

$(document).ready(function(){
	$('.contact').click(function(){
		$('#boxcontact').addClass('bigboxcontact');
	});
	$('.login').click(function(){
		$('#boxlogin').addClass('bigboxlogin');
	});
	$('.cta').click(function(){
		$('.cta').addClass('hide');
		$('.ctabox').addClass('bigctabox');
	});
});
	</script>

