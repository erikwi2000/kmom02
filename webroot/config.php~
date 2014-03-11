<?php
/**
 * Config-file for BWi. Change settings here to affect installation.
 *
 */

/**
 * Set the error reporting.
 *
 */
error_reporting(-1);              // Report all type of errors
ini_set('display_errors', 1);     // Display all errors 
ini_set('output_buffering', 0);   // Do not buffer outputs, write directly


/**
 * Define BWi paths.
 *
 */
define('BWI_INSTALL_PATH', __DIR__ . '/..');
define('BWI_THEME_PATH', BWI_INSTALL_PATH . '/theme/render.php');


/**
 * Include bootstrapping functions.
 *
 */
include(BWI_INSTALL_PATH . '/src/bootstrap.php');


/**
 * Start the session.
 *
 */
session_name(preg_replace('/[^a-z\d]/i', '', __DIR__));
session_start();


/**
 * Create the BWi variable.
 *
 */
$bwix = array();


/**
 * Site wide settings.
 *
 */
$bwix['lang']         = 'sv';
$bwix['title_append'] = ' | BWi en webbtemplate';

$bwix['header'] = <<<EOD
<img class='sitelogo' src='img/Anax.png' alt='BWi Logo'/>
<span class='sitetitle'>BWi webbtemplate</span>
<span class='siteslogan'>Återanvändbara moduler för webbutveckling med PHP</span>
EOD;

$bwix['footer'] = <<<EOD
<footer><span class='sitefooter'>Copyright (c) Mikael Roos (me@mikaelroos.se) | <a href='https://github.com/mosbth/BWi-base'>BWi på GitHub</a> | <a href='http://validator.w3.org/unicorn/check?ucn_uri=referer&amp;ucn_task=conformance'>Unicorn</a></span></footer>
EOD;



/**
 * Theme related settings.
 *
 */
//$bwix['stylesheet'] = 'css/style.css';
$bwix['stylesheets'] = array('css/style.css');
$bwix['favicon']    = 'favicon7.ico';



/**
 * Settings for JavaScript.
 *
 */
$bwix['modernizr'] = 'js/modernizr.js';

$bwix['jquery'] = '//ajax.googleapis.com/ajax/libs/jquery/1.10.1/jquery.min.js';
//$bwix['jquery'] = null; // To disable jQuery
$bwix['javascript_include'] = array();
//$bwix['javascript_include'] = array('js/main.js'); // To add extra javascript files
//echo "Helllloo";


/**
 * Google analytics.
 *
 */
$bwix['google_analytics'] = 'UA-22093351-1'; // Set to null to disable google analytics
