(function($) {
	
	"use strict";
	
	
	//Hide Loading Box (Preloader)
	function handlePreloader() {
		if($('.preloader').length){
			$('.preloader').delay(500).fadeOut(500);
		}
	}
	
	
	//Update Header Style + Scroll to Top
	function headerStyle() {
		if($('.main-header').length){
			var topHeader = $('.header-top').innerHeight();
			var windowpos = $(window).scrollTop();
			if (windowpos >= topHeader) {
				$('.main-header').addClass('fixed-top-header');
				$('.scroll-to-top').fadeIn(300);
			} else {
				$('.main-header').removeClass('fixed-top-header');
				$('.scroll-to-top').fadeOut(300);
			}
		}
	}
	if($('.main-header').length){
		var topHeader = $('.header-top').innerHeight();
		var windowpos = $(window).scrollTop();
		if (windowpos >= topHeader) {
			$('.main-header').addClass('fixed-top-header');
			$('.scroll-to-top').fadeIn(300);
		} else {
			$('.main-header').removeClass('fixed-top-header');
			$('.scroll-to-top').fadeOut(300);
		}
	}

	if ($('.thm-spinner').length) {
		var spinnerMin = $('.thm-spinner').data('min-value');
		var spinnerMax = $('.thm-spinner').data('max-value');
		var spinnerDefault = $('.thm-spinner').data('default-value');
		$('.thm-spinner').slider({
			range: 'min',
			min: spinnerMin,
			max: spinnerMax,
			value: spinnerDefault,
			slide: function( event, ui ) {
				$( '.vehicle-year' ).val( ui.value );
			}
		});
		$( '.vehicle-year' ).val( $('.thm-spinner').slider('value') );
	};

	if ($('.select-input').length) {
		$('.select-input').selectmenu();
	};
	if ($('.date-picker').length) {
		$('.date-picker').datepicker();
	};

	if ($('ul.special-checkbox').length) {
		$('ul.special-checkbox').find('li').on('click', function () {
			$(this).toggleClass('active');
			// toggling checkbox with click event
			$(this).find('input[type=checkbox]').prop('checked', function(){
				return !this.checked;
			});
		});		
	};	
	
	
	//Submenu Dropdown Toggle
	if($('.main-header li.dropdown .submenu').length){
		$('.main-header li.dropdown').append('<div class="dropdown-btn"></div>');
		
		//Dropdown Button
		$('.main-header li.dropdown .dropdown-btn').on('click', function() {
			$(this).prev('.submenu').slideToggle(500);
		});
	}
	
	
	//Main Slider
	if($('.main-slider').length){

		jQuery('.tp-banner').show().revolution({
		  delay:7500,
		  startwidth:1200,
		  startheight:620,
		  hideThumbs:600,
	
		  thumbWidth:80,
		  thumbHeight:50,
		  thumbAmount:5,
	
		  navigationType:"bullet",
		  navigationArrows:"1",
		  navigationStyle:"preview4",
	
		  touchenabled:"on",
		  onHoverStop:"off",
	
		  swipe_velocity: 0.7,
		  swipe_min_touches: 1,
		  swipe_max_touches: 1,
		  drag_block_vertical: false,
	
		  parallax:"mouse",
		  parallaxBgFreeze:"on",
		  parallaxLevels:[7,4,3,2,5,4,3,2,1,0],
	
		  keyboardNavigation:"on",
	
		  navigationHAlign:"center",
		  navigationVAlign:"bottom",
		  navigationHOffset:0,
		  navigationVOffset:20,
	
		  soloArrowLeftHalign:"left",
		  soloArrowLeftValign:"center",
		  soloArrowLeftHOffset:20,
		  soloArrowLeftVOffset:0,
	
		  soloArrowRightHalign:"right",
		  soloArrowRightValign:"center",
		  soloArrowRightHOffset:20,
		  soloArrowRightVOffset:0,
	
		  shadow:0,
		  fullWidth:"on",
		  fullScreen:"off",
	
		  spinner:"spinner4",
	
		  stopLoop:"off",
		  stopAfterLoops:-1,
		  stopAtSlide:-1,
	
		  shuffle:"off",
	
		  autoHeight:"off",
		  forceFullWidth:"on",
	
		  hideThumbsOnMobile:"on",
		  hideNavDelayOnMobile:1500,
		  hideBulletsOnMobile:"on",
		  hideArrowsOnMobile:"on",
		  hideThumbsUnderResolution:0,
	
		  hideSliderAtLimit:0,
		  hideCaptionAtLimit:0,
		  hideAllCaptionAtLilmit:0,
		  startWithSlide:0,
		  videoJsPath:"",
		  fullScreenOffsetContainer: ".main-slider"
	  });

		
	}
	
	
	//Tabs Box
	if($('.tabs-box').length){
		$('.tabs-box .tab-btn').on('click', function(e) {
			e.preventDefault();
			var target = $($(this).attr('href'));
			$('.tabs-box .tab-btn').removeClass('active-btn');
			$(this).addClass('active-btn');
			$('.tabs-box .tab').fadeOut(0);
			$('.tabs-box .tab').removeClass('active-tab');
			$(target).fadeIn(300);
			$(target).addClass('active-tab');
			var windowWidth = $(window).width();
			if (windowWidth <= 700) {
				$('html, body').animate({
				   scrollTop: $('.tabs-box .tabs-content').offset().top
				 }, 1000);
			}
		});
		
	}
	
	
	//Four Column Slider
	if ($('.column-carousel.four-column').length) {
		$('.column-carousel.four-column').owlCarousel({
			loop:true,
			margin:30,
			nav:true,
			autoplayHoverPause:true,
			autoplay: 5000,
			smartSpeed: 1000,
			responsive:{
				0:{
					items:1
				},
				600:{
					items:2
				},
				800:{
					items:2
				},
				1024:{
					items:3
				},
				1100:{
					items:4
				}
			}
		});    		
	}
	
	
	//Three Column Slider
	if ($('.column-carousel.three-column').length) {
		$('.column-carousel.three-column').owlCarousel({
			loop:true,
			margin:30,
			nav:true,
			autoplayHoverPause:false,
			autoplay: 5000,
			smartSpeed: 700,
			responsive:{
				0:{
					items:1
				},
				600:{
					items:2
				},
				800:{
					items:2
				},
				1024:{
					items:3
				},
				1100:{
					items:3
				}
			}
		});    		
	}
	
	//Two Column Slider
	if ($('.column-carousel.two-column').length) {
		$('.column-carousel.two-column').owlCarousel({
			loop:true,
			margin:30,
			nav:true,
			autoplayHoverPause:false,
			autoplay: 5000,
			smartSpeed: 1000,
			responsive:{
				0:{
					items:1
				},
				600:{
					items:1
				},
				800:{
					items:2
				},
				1024:{
					items:2
				},
				1100:{
					items:2
				}
			}
		});    		
	}
	
	
	
	//Sponsors Slider
	if ($('.sponsors .slider').length) {
		$('.sponsors .slider').owlCarousel({
			loop:true,
			margin:20,
			nav:true,
			autoplay: 5000,
			responsive:{
				0:{
					items:1
				},
				600:{
					items:2
				},
				800:{
					items:3
				},
				1024:{
					items:4
				},
				1100:{
					items:5
				}
			}
		});    		
	}
	
	
	//LightBox / Fancybox
	if($('.lightbox-image').length) {
		$('.lightbox-image').fancybox();
	}
	
	
	//Vertical Gallery Slider
	if ($('.vertical-gallery').length) {
		var slider = new MasterSlider();
		slider.setup('vertical-gallery' , {
			autoplay:true,
			loop:true,
			width:870,
			height:530,
			space:5,
			view:'basic',
			dir:'h'
		});
		slider.control('arrows');	
		slider.control('scrollbar' , {dir:'h'});	
		slider.control('circletimer' , {color:"#FFFFFF" , stroke:9});
		slider.control('thumblist' , {autohide:false ,dir:'v'});  		
	}
	
	
	//Filters Section / Mixitup
	if($('.filter-list').length){
		$('.filter-list').mixitup({});
	}
	
	
	//Contact Form Validation
	if($('#contact-form').length){
		//------------
	}
	
	// Scroll to top
	if($('.scroll-to-top').length){
		$(".scroll-to-top").on('click', function() {
		   // animate
		   $('html, body').animate({
			   scrollTop: $('html, body').offset().top
			 }, 1000);
	
		});
	}
	
	
	// Elements Animation
	if($('.wow').length){
		var wow = new WOW(
		  {
			boxClass:     'wow',      // animated element css class (default is wow)
			animateClass: 'animated', // animation css class (default is animated)
			offset:       0,          // distance to the element when triggering the animation (default is 0)
			mobile:       true,       // trigger animations on mobile devices (default is true)
			live:         true       // act on asynchronously loaded content (default is true)
		  }
		);
		wow.init();
	}

/* ==========================================================================
   When document is ready, do
   ========================================================================== */
   
	$(document).on('ready', function() {
		headerStyle();
	});

/* ==========================================================================
   When document is Scrollig, do
   ========================================================================== */
	
	$(window).on('scroll', function() {
		headerStyle();
	});
	
/* ==========================================================================
   When document is loading, do
   ========================================================================== */
	
	$(window).on('load', function() {
		handlePreloader();
	});
	

})(window.jQuery);
/*----------------------------
		contact form 
-----------------------------*/
jQuery(document).ready(function($) {			   
		
		$('#contact-form').submit(function(){

			var action = $(this).attr('action');
	
			$("#message").slideUp(750,function() {
			$('#message').hide();
	
			$('button#submit').attr('disabled','disabled');
			$('img.loader').css('visibility', 'visible');
	
			$.post(action, {
				contact_name: $('#contact_name').val(),
				contact_email: $('#contact_email').val(),
				contact_subject: $('#contact_subject').val(),
				contact_message: $('#contact_message').val(),
				verify: $('#verify').val()
			},
				function(data){
					document.getElementById('message').innerHTML = data;
					$('#message').slideDown('slow');
					$('#contactform img.loader').css('visibility', 'hidden' );
					
					$('#submit').removeAttr('disabled');
					if(data.match('success') != null) $('#contactform').slideUp('slow');
	
				}
			);

		});

		return false;

	});
	
	//----widget contact form
	
			$('#footer_contact-form').submit(function(){

			var action = $(this).attr('action');
	
			$("#footer_message").slideUp(750,function() {
			$('#footer_message').hide();
	
			$('button#submit').attr('disabled','disabled');
			$('img.loader').css('visibility', 'visible');
	
			$.post(action, {
				footer_contact_name: $('#footer_contact_name').val(),
				footer_contact_email: $('#footer_contact_email').val(),
				footer_contact_message: $('#footer_contact_message').val(),
				verify: $('#verify').val()
			},
				function(data){
					document.getElementById('footer_message').innerHTML = data;
					$('#footer_message').slideDown('slow');
					$('#contactform img.loader').css('visibility', 'hidden' );
					
					$('#submit').removeAttr('disabled');
					if(data.match('success') != null) $('#contactform').slideUp('slow');
	
				}
			);

		});

		return false;

	});
	 // appointment-form
	$('#appointment_form').submit(function(){
		
		   var action = $(this).attr('action');
		 
		   $("#apt_message").slideUp(750,function() {
		   $('#apt_message').hide();
		 
		   $('button#submit').attr('disabled','disabled');
		   $('img.loader').css('visibility', 'visible');
		
		
		
		var chkboxArray = [];
		$("input:checkbox[name=apt_vehicle_services_needed]:checked").each(function() {
			chkboxArray.push(this.value);
		});
		
		
		
		   $.post(action, {
		 
			apt_vehicle_year: $('#apt_vehicle_year').val(),
			apt_vehicle_make: $('#apt_vehicle_make').val(),
			apt_vehicle_milage: $('#apt_vehicle_milage').val(),
			apt_date: $('#apt_date').val(),
			apt_timeframe: $('#apt_timeframe').val(),
			apt_customer_name: $('#apt_customer_name').val(),
			apt_customer_email: $('#apt_customer_email').val(),
			apt_customer_subject: $('#apt_customer_subject').val(),
			apt_customer_message: $('#apt_customer_message').val(),
			receiver_email: $('#receiver_email').val(),
			apt_vehicle_services_needed : chkboxArray
		},
			function(data){
			 document.getElementById('apt_message').innerHTML = data;
			 $('#apt_message').slideDown('slow');
			 $('#appointment_form img.loader').css('visibility', 'hidden' );
			 
			 $('#submit').removeAttr('disabled');
			 if(data.match('success') != null) $('#appointment_form').slideUp('slow');
		 
			}
		   );
		
		  });
		
		  return false;
		
		 });
		
		
	});