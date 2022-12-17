<?php

/**
 * The header for our theme
 *
 * This is the template that displays all of the <head> section and everything up until <div id="content">
 *
 * @link https://developer.wordpress.org/themes/basics/template-files/#template-partials
 *
 * @package WordPress
 * @subpackage Twenty_Seventeen
 * @since Twenty Seventeen 1.0
 * @version 1.0
 */
error_reporting(0);
?>
<!DOCTYPE html>
<html <?php language_attributes(); ?> class="no-js no-svg">

<head>
    <meta charset="<?php bloginfo('charset'); ?>">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="profile" href="https://gmpg.org/xfn/11">

    <?php wp_head(); ?>
    <!-- Google Tag Manager -->

    <script>
        (function(w, d, s, l, i) {
            w[l] = w[l] || [];
            w[l].push({
                'gtm.start':

                    new Date().getTime(),
                event: 'gtm.js'
            });
            var f = d.getElementsByTagName(s)[0],

                j = d.createElement(s),
                dl = l != 'dataLayer' ? '&l=' + l : '';
            j.async = true;
            j.src =

                'https://www.googletagmanager.com/gtm.js?id=' + i + dl;
            f.parentNode.insertBefore(j, f);

        })(window, document, 'script', 'dataLayer', 'GTM-5TB34J6');
    </script>

    <!-- End Google Tag Manager -->
</head>

<body <?php body_class(); ?>>
    <!-- Google Tag Manager (noscript) -->

    <noscript>
        <iframe src="https://www.googletagmanager.com/ns.html?id=GTM-5TB34J6" height="0" width="0" style="display:none;visibility:hidden"></iframe>
    </noscript>

    <!-- End Google Tag Manager (noscript) -->

    <?php wp_body_open(); ?>
    <!--start header-->
    <header class="full-width main_head navbar-fixed-top" id="header">
        <div class="cov_19">
            <?php
            $covide_resources_text =  get_field('covid_resource', 'options');
            if ($covide_resources_text) {
                echo $covide_resources_text;
            }
            ?>
        </div>
        <?php /*
<!--    <div class="logo_sec <?php if(is_page('contact-us')) { echo "contact-page";}?>"> -->
<!-- <div class="logo_sec <?php if(is_page('contact-us')) { echo "contact-page";}?>" <?php if(is_page('contact-us')) { ?> style="background-image: url(<?php echo get_stylesheet_directory_uri(); ?>/images/abtindividualbnr.webp),url(<?php echo get_stylesheet_directory_uri(); ?>/images/abtindividualbnr.jpg;" <?php } ?>> -->
*/ ?>
        <?php if (is_page('contact-us')) { ?>
            <div style="clear:both"></div>
            <div class="logo_sec" style="background-image: url(<?php echo get_stylesheet_directory_uri(); ?>/images/abtindividualbnr.webp),url(<?php echo get_stylesheet_directory_uri(); ?>/images/abtindividualbnr.jpg;">
            <?php } else { ?>
                <div class="container-fluid" style="background:#fff">

                    <div class="container">
                        <div class="row py-3">
                            <div class="col-md-8  "><?php $logo =  get_field('logo', 'options');
                                                                if ($logo) { ?>
                                    <a href="<?php echo home_url(); ?>"><img src="https://wordpress-374901-2912333.cloudwaysapps.com/wp-content/uploads/2022/09/logo-black.png" width="372px" alt="brar_logo"></a>
                                <?php } else { ?>
                                    <a href="<?php echo home_url(); ?>"><img src="https://wordpress-374901-2912333.cloudwaysapps.com/wp-content/uploads/2022/09/logo-black.png" width="372px" alt="brar_logo"></a>
                                <?php } ?>
                            </div>
                            <div class="col-md-4 ">
                                <h1>
                                     
                                        <img src="https://wordpress-374901-2912333.cloudwaysapps.com/wp-content/uploads/2022/09/Vector-8.png">
                                    

                                    <span style="color:#6C6C6C;     Font-family: Roboto;    Font-style: Light;  Font-size: 36px;         font-Weight:300;
                                                        Line-height: 42px">

                                        1-833-</span>
                                    <span style="color:#3893D5;
                                                         font-Weight:300;
                                                        Font-family: Roboto;
                                                        Font-style: Light;
                                                        Font-size: 36px;
                                                        Line-height: 42px">
                                        BRAR-LAW </span>
                                </h1>
                                <p class="mt-2 mx-5" style="Font-family: Roboto;
                                   color:#6C6C6C; Font-style: Bold;Font-size: 16px;
                                   margin-right:30px;
                                   font-weight:700;Line-height: 19px;text-align: center; margin-right: 140px !important;">
                                    Call us 24/7
                                </p>
                            </div>
                        </div>
                    </div>
                </div>

				<div class="call-button">
					<div class="call-button-section-1">
						<div style="margin-bottom:4px;margin-left: 7px;"><img width="17px" height="17px" src="https://wordpress-374901-2912333.cloudwaysapps.com/wp-content/uploads/2022/09/Vector-8.png"><span style='letter-spacing: 2px;margin-left:5px;font-size:16px;color:#6C6C6C;font-weight:300;Font-family:Roboto'>1-833-<span style="color:#3893D5;font-weight:400;Font-family:Roboto">BRAR-LAW </span></span>
						</div>
						<div style="color:#6C6C6C;Font-family: Roboto;Font-style:Bold;Font-size:10px;Line-height:12px;font-weight:700;"> Call us 24/7 to book a free consultation 	</div>
					</div>
					<div>
					<button type="button" class="nav-mob-btn" href="https://www.brartamber.com/book-a-consultation/">book a free consultation</button>
						
					</div>
				</div>
				<hr>
                <div class="logo_sec">
                <?php } ?>
                <div class="container">
						
                    <div class="brar_menu navigation">
						<div class="mobile-logo">
							<img src="https://wordpress-374901-2912333.cloudwaysapps.com/wp-content/uploads/2022/09/BRAR-TAMBER-RIGBY-LOGO-2-3.png">
						</div>
                        <div class="nav-bar">
                            <i class="fa fa-bars" id="mobnav" style="display: block;"></i>
                        </div>

                        <nav style="left: -100%;">
                            <i class="fa fa-times" id="cross" style="display: none;"></i>
                            <div class="mobile-logo">
                                <?php $logo =  get_field('logo', 'options');
                                if ($logo) { ?>
                                    <a href="<?php echo home_url(); ?>"><img src="<?php echo $logo; ?>" alt="brar_logo"></a>
                                <?php } else { ?>
                                    <a href="<?php echo home_url(); ?>"><img src="<?php echo get_stylesheet_directory_uri(); ?>/images/brar_logo.png" alt="brar_logo"></a>
                                <?php } ?>
                            </div>

                            <div class="menu-header-main-menu-container">
                                <?php if (has_nav_menu('top')) : ?>
                                    <?php wp_nav_menu(array('theme_location' => 'top', 'menu_id' => 'top', 'menu_class' => 'menu')); ?>
                                <?php endif; ?>
                            </div>

                            <div class="mobile-footer">
                                <ul>
                                    <li><span>Call Us:</span> Office: <a href="tel:+1<?php echo str_replace("-", "", get_field('phone', 'options'));  ?>"><?php echo get_field('phone', 'options'); ?></a> <br> Cell: <a href="tel:+1<?php echo str_replace("-", "", get_field('toll_free', 'options'));  ?>"><?php echo get_field('toll_free_only', 'options'); ?></a> </li>
                                    <li>
                                    </li>
                                    <li><span>Email:</span> <a href="mailto:<?php echo get_field('email', 'options'); ?>"><?php echo get_field('email', 'options'); ?></a></li>
                                </ul>
                            </div>

                        </nav>
                    </div>
                </div>
                </div>
            </div>
    </header>
    <!--end header-->
    <?php
    if (!is_page('contact-us')) {
        $counter = 1;
        if (is_front_page() && have_rows('home_banner', 'options')) {
    ?>

            <?php

            ?>
            <!--start banner-->
            <section class="full-width page_banner pt-5">
                <div class="multiple-items slider">
                    <?php while (have_rows('home_banner', 'options')) : the_row();
                        $webp_image = get_sub_field('webp_image', 'options');
                        $banner_img = get_sub_field('bimage', 'options');
                        $link_text = get_sub_field('link_text', 'options');
                        if ($link_text) {
                            $l_text = $link_text;
                        } else {
                            $l_text = 'Read more';
                        }
                    ?>
                        <div>
                            <div class="banner_panel">
                                <?php if ($banner_img) { ?>
                                    <?php /*<img src="<?php echo $banner_img; ?>" alt="banner_<?php echo $counter; ?>"> */ ?>
                                    <picture>
                                        <source srcset="<?php echo $webp_image; ?>" type="image/webp" alt="image">
                                        <source srcset="<?php echo $banner_img; ?>" type="image/jpeg" alt="banner_<?php echo $counter; ?>">
                                        <img src="<?php echo $banner_img; ?>" alt="banner_<?php echo $counter; ?>">
                                    </picture>
                                <?php } else { ?>
                                    <?php /*<img src="<?php echo get_stylesheet_directory_uri(); ?>/images/banner_1.jpg" alt="banner_<?php echo $counter; ?>"> */ ?>
                                    <picture>
                                        <source srcset="<?php echo get_stylesheet_directory_uri(); ?>/images/banner_1.webp" type="image/webp" alt="image">
                                        <source srcset="<?php echo get_stylesheet_directory_uri(); ?>/images/banner_1.jpg" type="image/jpeg" alt="banner_<?php echo $counter; ?>">
                                        <img src="<?php echo get_stylesheet_directory_uri(); ?>/images/banner_1.jpg" alt="banner_<?php echo $counter; ?>">
                                    </picture>
                                <?php } ?>

                                <div class="banner_text">
                                    <h2><?php echo get_sub_field('btitle', 'options'); ?></h2>
                                    <p><a href="<?php echo get_sub_field('blink', 'options'); ?>"><?php echo $l_text; ?></a></p>
                                </div>
                            </div>
                        </div>
                    <?php $counter++;
                    endwhile; ?>
                </div>
                <div class="hm_bnr_frm_bg" style="margin-top: 100px;">
                    <div class="hm_bnr_frm">
                        <h3>Book a free consultation</h3>
                        <?php echo do_shortcode('[contact-form-7 id="1270" title="Book A Consultation"]'); ?>
                    </div>
                </div>
            </section>


            <?php //} 
            ?>
            <!--end banner-->
        <?php } else if (is_singular('partner')) {
            $bnr_img =  get_field('banner_image', $post->ID);
            $webp_banner_image =  get_field('webp_banner_image', $post->ID);

            if ($bnr_img) {
                $banner_image = $bnr_img;
                $banner_image_webp = $webp_banner_image;
            } else {
                $banner_image = get_stylesheet_directory_uri() . '/images/abtbnr.jpg';
                $banner_image_webp = get_stylesheet_directory_uri() . '/images/abtbnr.webp';
            } ?>
            <!-- start banner -->
            <!--    <section class="full-width abtindividualbnr" style="background-image: url(<?php echo $banner_image; ?>"> -->
            <section class="full-width abtindividualbnr" style="background-image:url(<?php echo $banner_image_webp; ?>),url(<?php echo $banner_image; ?>;">

            </section>
        <?php } else if (is_singular('staff')) {
            $bnr_img =  get_field('banner_image', $post->ID);
            $webp_banner_image =  get_field('webp_banner_image', $post->ID);
            if ($bnr_img) {
                $banner_image = $bnr_img;
                $banner_image_webp = $webp_banner_image;
            } else {
                $banner_image = get_stylesheet_directory_uri() . '/images/abtbnr.jpg';
                $banner_image_webp = get_stylesheet_directory_uri() . '/images/abtbnr.webp';
            } ?>
            <!-- start banner -->
            <!-- <section class="full-width abtindividualbnr" style="background-image: url(<?php echo $banner_image; ?>"> -->
            <section class="full-width abtindividualbnr" style="background-image:url(<?php echo $banner_image_webp; ?>),url(<?php echo $banner_image; ?>;">
            </section>

        <?php } else if (is_page_template('page-templates/service-details-template.php')) {
            $bnr_img =  get_field('banner_image', $post->ID);
            $webp_banner_image =  get_field('webp_banner_image', $post->ID);
            if ($bnr_img) {
                $banner_image = $bnr_img;
                $banner_image_webp = $webp_banner_image;
            } else {
                $banner_image = get_stylesheet_directory_uri() . '/images/abtbnr.jpg';
                $banner_image_webp = get_stylesheet_directory_uri() . '/images/abtbnr.webp';
            } ?>
            <!--    <section class="full-width servicebnr" style="background-image: url(<?php echo $banner_image; ?>);"> -->
            <section class="full-width abtindividualbnr" style="background-image:url(<?php echo $banner_image_webp; ?>),url(<?php echo $banner_image; ?>;">
                <div class="srvcbnrcntnt">
                    <h1><?php echo get_post_field('post_title', $post->ID); ?></h1>
                </div>
            </section>
        <?php } else if (!is_front_page() && is_home()) {   ?>
            <section class="full-width mb_60">
                <div class="abtbnr">
                    <?php
                    global $post;
                    $post_id =  get_option('page_for_posts');
                    $bnr_img =  get_field('banner_image', $post_id);
                    $webp_banner_image =  get_field('webp_banner_image', $post_id);
                    ?>
                    <?php if ($bnr_img) { ?>
                        <!-- <img src="<?php echo $bnr_img; ?>" alt="banner-<?php echo $post->ID; ?>"> -->
                        <picture>
                            <source srcset="<?php echo $webp_banner_image; ?>" type="image/webp" alt="banner-<?php echo $post->ID; ?>">
                            <source srcset="<?php echo $bnr_img; ?>" type="image/jpeg" alt="banner-<?php echo $post->ID; ?>">
                            <img src="<?php echo $bnr_img; ?>" alt="banner-<?php echo $post->ID; ?>">
                        </picture>
                    <?php } else { ?>
                        <!--    <img src="<?php echo get_stylesheet_directory_uri(); ?>/images/abtbnr.jpg" alt="#"> -->
                        <picture>
                            <source srcset="<?php echo get_stylesheet_directory_uri(); ?>/images/abtbnr.webp" type="image/webp" alt="banner">
                            <source srcset="<?php echo get_stylesheet_directory_uri(); ?>/images/abtbnr.jpg" type="image/jpeg" alt="banner">
                            <img src="<?php echo get_stylesheet_directory_uri(); ?>/images/abtbnr.jpg" alt="banner">
                        </picture>
                    <?php } ?>
                </div>
            </section>
        <?php } else if (is_404()) {
            $bnr_img =  get_field('banner_image', $post->ID);
            if ($bnr_img) {
                $banner_image = $bnr_img;
            } else {
                $banner_image = get_stylesheet_directory_uri() . '/images/abtbnr.jpg';
            } ?>
            <section class="full-width servicebnr" style="background-image: url(<?php echo $banner_image; ?>);">
                <div class="srvcbnrcntnt">
                    <h1>404 : Page not found</h1>
                </div>
            </section>
        <?php } else if (is_page('practice-areas')) {
            $page_featured_image_url = wp_get_attachment_url(get_post_thumbnail_id($post->ID));
            $webp_banner_image =  get_field('webp_banner_image', $post->ID);
            if ($page_featured_image_url) {
                $banner_image = $page_featured_image_url;
                $banner_image_webp = $webp_banner_image;
            } else {
                $banner_image = get_stylesheet_directory_uri() . '/images/abtbnr.jpg';
                $banner_image_webp = get_stylesheet_directory_uri() . '/images/abtbnr.webp';
            }

        ?>

            <!--    <section class="full-width servicebnr" style="background-image: url(<?php echo $banner_image; ?>);"> -->
            <section class="full-width servicebnr" style="background-image:url(<?php echo $banner_image_webp; ?>),url(<?php echo $banner_image; ?>;">
                <div class="srvcbnrcntnt">
                    <h1><?php echo get_the_title($post->ID); ?></h1>
                </div>
            </section>

        <?php } else if (is_page_template('page-templates/template-faq.php')) {
            //$page_featured_image_url = wp_get_attachment_url( get_post_thumbnail_id($post->ID) );
            $page_featured_image_url =  get_field('banner_image', $post->ID);
            $webp_banner_image =  get_field('webp_banner_image', $post->ID);
            if ($page_featured_image_url) {
                $banner_image = $page_featured_image_url;
                $banner_image_webp = $webp_banner_image;
            } else {
                $banner_image = get_stylesheet_directory_uri() . '/images/abtbnr.jpg';
                $banner_image_webp = get_stylesheet_directory_uri() . '/images/abtbnr.webp';
            }
            $banner_heading = get_field('banner_heading', $post->ID);
        ?>

            <!-- <section class="full-width servicebnr" style="background-image: url(<?php echo $banner_image; ?>);"> -->
            <section class="full-width servicebnr" style="background-image:url(<?php echo $banner_image_webp; ?>),url(<?php echo $banner_image; ?>;">
                <div class="srvcbnrcntnt">
                    <h1><?php echo $banner_heading; ?></h1>
                </div>
            </section>
        <?php } else if (is_tax()) {
            $taxonomy_object = get_queried_object();
            $taxonomy_id = $taxonomy_object->term_id;
            $page_featured_image_url = get_field('banner_image', $taxonomy . '_' . $taxonomy_id);
            $page_featured_image_url_webp = get_field('banner_image_webp', $taxonomy . '_' . $taxonomy_id);
            if ($page_featured_image_url) {
                $banner_image = $page_featured_image_url['url'];
                $banner_image_webp = $page_featured_image_url_webp['url'];
            } else {
                $banner_image = get_stylesheet_directory_uri() . '/images/abtbnr.jpg';
                $banner_image_webp = get_stylesheet_directory_uri() . '/images/abtbnr.webp';
            }
            $banner_heading = get_field('banner_heading', $post->ID);
        ?>

            <section class="full-width servicebnr" style="background-image: url(<?php echo $banner_image_webp; ?>),url(<?php echo $banner_image; ?>;">
                <div class="srvcbnrcntnt">
                    <h1><?php echo $taxonomy_object->name; ?></h1>
                </div>
            </section>

        <?php } else if (is_singular('practice-area')) { ?>


        <?php }  else if (is_page_template('page-templates/about-page.php')) { ?>

            <section class="full-width mb_60" style="display: none">
                    <div class="abtbnr">
                        <?php $bnr_img =  get_field('banner_image', $post->ID);
                        $webp_banner_image =  get_field('webp_banner_image', $post->ID);
                        ?>
                        <?php if ($bnr_img) { ?>
                            <!-- <img src="<?php echo $bnr_img; ?>" alt="banner-<?php echo $post->ID; ?>"> -->
                            <picture>
                                <source srcset="<?php echo $webp_banner_image; ?>" type="image/webp" alt="banner-<?php echo $post->ID; ?>">
                                <source srcset="<?php echo $bnr_img; ?>" type="image/jpeg" alt="banner-<?php echo $post->ID; ?>">
                                <img src="<?php echo $bnr_img; ?>" alt="banner-<?php echo $post->ID; ?>">
                            </picture>
                        <?php } else { ?>
                            <!-- <img src="<?php echo get_stylesheet_directory_uri(); ?>/images/abtbnr.jpg" alt="#"> -->
                            <picture>
                                <source srcset="<?php echo get_stylesheet_directory_uri(); ?>/images/abtbnr.webp" type="image/webp" alt="banner">
                                <source srcset="<?php echo get_stylesheet_directory_uri(); ?>/images/abtbnr.jpg" type="image/jpeg" alt="banner">
                                <img src="<?php echo get_stylesheet_directory_uri(); ?>/images/abtbnr.jpg" alt="banner">
                            </picture>
                        <?php }  ?>
                    </div>
                </section>


     <?php   } else { ?>
            <!--start banner-->
            <?php if (!is_page_template('page-templates/page-landing-four.php') && !is_page_template('page-templates/page-landing-two.php') && !is_page_template('page-templates/page-landing.php') && !is_page_template('page-templates/page-landing-three.php') && !is_page_template('page-templates/page-landing-five.php') && !is_page_template('page-templates/page-landing-six.php')) {
            ?>
                <section class="full-width mb_60" style="display: none">
                    <div class="abtbnr">
                        <?php $bnr_img =  get_field('banner_image', $post->ID);
                        $webp_banner_image =  get_field('webp_banner_image', $post->ID);
                        ?>
                        <?php if ($bnr_img) { ?>
                            <!-- <img src="<?php echo $bnr_img; ?>" alt="banner-<?php echo $post->ID; ?>"> -->
                            <picture>
                                <source srcset="<?php echo $webp_banner_image; ?>" type="image/webp" alt="banner-<?php echo $post->ID; ?>">
                                <source srcset="<?php echo $bnr_img; ?>" type="image/jpeg" alt="banner-<?php echo $post->ID; ?>">
                                <img src="<?php echo $bnr_img; ?>" alt="banner-<?php echo $post->ID; ?>">
                            </picture>
                        <?php } else { ?>
                            <!-- <img src="<?php echo get_stylesheet_directory_uri(); ?>/images/abtbnr.jpg" alt="#"> -->
                            <picture>
                                <source srcset="<?php echo get_stylesheet_directory_uri(); ?>/images/abtbnr.webp" type="image/webp" alt="banner">
                                <source srcset="<?php echo get_stylesheet_directory_uri(); ?>/images/abtbnr.jpg" type="image/jpeg" alt="banner">
                                <img src="<?php echo get_stylesheet_directory_uri(); ?>/images/abtbnr.jpg" alt="banner">
                            </picture>
                        <?php }  ?>
                    </div>
                </section>
                <!--end banner-->
    <?php }
        }
    } ?>

    <?php //if ( is_front_page() && is_home() )
    if (!is_front_page() && !is_page_template('page-templates/page-landing-four.php') && !is_page_template('page-templates/page-landing-two.php') && !is_page_template('page-templates/page-landing.php') && !is_page_template('page-templates/page-landing-three.php') && !is_page_template('page-templates/page-landing-five.php') && !is_page_template('page-templates/page-landing-six.php') && !is_singular('practice-area')) {
        //echo 'sssssssss';
        if (function_exists('yoast_breadcrumb')) {
            yoast_breadcrumb('<p id="breadcrumbs">', '</p>');
        }
    } ?>