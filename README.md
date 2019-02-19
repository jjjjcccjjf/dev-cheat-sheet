# Dev Cheat Sheet 👻😵🙃
Just a compilation of kick-ass tools and code snippets to kickstart your development mostly for web and APIs. Contributions are open!

    “Never memorize something that you can look up.”

    ― Albert Einstein

# TODO:
* Add cute emojis
* Add frameworks
    * Codeigniter
    * Laravel
* Add PHP & Web references
* Add REST Crud
* jp_lib
* __Add back to top__

---
 
# Contents 
#### Development Tools
* [Text Editors / Integrated Development Environment (IDE)](#text-editors--integrated-development-environment-ide)
    * [Atom](https://atom.io/)
    * [Sublime Text](https://www.sublimetext.com/)
    * [Visual Studio Code](https://code.visualstudio.com/)
* [Chrome Extensions](#chrome-extensions)
    * [var_masterpiece](https://chrome.google.com/webstore/detail/varmasterpiece/chfhddogiigmfpkcmgfpolalagdcamkl?utm_source=chrome-app-launcher-info-dialog)
    * [JSON Formatter](https://chrome.google.com/webstore/detail/bcjindcccaagfpapjjmafapmmgkkhgoa?utm_source=chrome-app-launcher-info-dialog)
    * [Postman](https://chrome.google.com/webstore/detail/postman/fhbjgbiflinjbdggehcddcbncdddomop?hl=en)
* File Transfer Clients
   * [FIlezilla](https://filezilla-project.org/)
* [Version Control Clients](#version-control-clients)
   * [SourceTree](https://www.sourcetreeapp.com/)
   * [Git Kraken](https://www.gitkraken.com/)
* Other Tools
   * [Git Bash (Terminal Interface)](https://git-scm.com/downloads)
#### Standards
* [PHP Standard Recommendations (PSR)](http://www.php-fig.org/psr/)
* [RESTful APIs](http://www.restapitutorial.com/)
#### Code Snippets
* [Front-end](#front-end)
    * [CSS Snippets](#css-snippets)
    * [Animation Snippets](#animation-snippets)
* [Back-end](#back-end)
    * [PHP Snippets](#php-snippets)
        * [Wordpress](#wordpress)
            * [Installing Wordpress](#installing-wordpress)
            * [Branding your theme](#branding-your-theme)
            * [Common wordpress plugins](#common-wordpress-plugins)
            * [Wordpress Snippets](#wordpress-snippets)
            * [Var dump information / Common WP Object / Array structures](#tired-of-var_dump-ing-heres-some-common-wp-objectarray-structures)
        * Generic PHP Snippets
    * JavaScript Snippets
    * [REST-Igniter Authorization](#rest-igniter-authorization)
    * [Accelerated Mobile Pages (AMP)](#accelerated-mobile-pages-amp)
* Other
    * [ReCAPTCHA Code Snippet](https://www.google.com/url?q=https://gist.github.com/jjjjcccjjf/bb5f0053244a431ba5bc60ee1943c38b&sa=D&source=hangouts&ust=1524816959016000&usg=AFQjCNGfwqQujYlLQgvFuULV_dXIHUcffQ)
* [Pen Test Countermeasures](https://gist.github.com/jjjjcccjjf/30c5b818b2f7d33e753d8b8a5d16dd0a)
    
#### API
* [Twitter API](#twitter-api)
* [TwitterOAuth PHP Library for the Twitter REST API](https://twitteroauth.com/)

#### Deployment
* [Command-line snippets](#command-line-snippets)
    * [Installing Wordpress](#installing-wordpress)
    * [Setup your version control](#setup-your-version-control)
* [.htaccess](#htaccess)
    * [Leverage browser caching](#leverage-browser-caching)
#### Cheat sheets & References
* [Git Cheatsheet](https://github.com/jjjjcccjjf/dev-cheat-sheet/blob/master/cheat-sheets/git-cheat-sheet.md)
* [Markdown Cheatsheet](https://github.com/jjjjcccjjf/dev-cheatsheet/blob/master/cheat-sheets/markdown-cheat-sheet.md)
* [Regular Expressions (RegEx)](https://github.com/zeeshanu/learn-regex)
* [Git commit conventions](https://chris.beams.io/posts/git-commit/)
* [.gitignore for Wordpress](https://gist.github.com/jjjjcccjjf/7516920786f200414d0178d7bcdaf06f)
* [WP Optimize Guide](https://github.com/jjjjcccjjf/wp-optimize-guide/blob/master/README.md)
- - -

# Development Tools

## Text Editors / Integrated Development Environment (IDE)
[⬆ Back to top](#dev-cheat-sheet-)

## Atom
What I like about atom is its IDE-like experience and it also has a lot of nice plugins that I really think is essential for an efficient development workflow. This is my preffered Text Editor as well.
#### Pros:
* Packages
* Has an interface for installing packages and themes, etc
* Almost like an IDE
* Has built-in GIT integration
#### Cons:
*  Slow to boot
*  Unresponsive bug
#### Recommended Packages
* Remote FTP
* Markdown Previewer Plus
* docblockr
* jquery-snippets

[View Website](https://atom.io/)

## Sublime Text
I don't use sublime that much but it's blazingly fast compared to other text editors.
#### Pros:
* Super fast
#### Cons: 
* Installing packages is such a hassle
#### Recommended Packages:
* TODO:

[View Website](https://www.sublimetext.com/)
## Visual Studio Code
Haven't used this much yet. So I don't have much opinion about it.

[View Website](https://code.visualstudio.com/)

- - -
# Chrome Extensions
[⬆ Back to top](#dev-cheat-sheet-)

## var_masterpiece
For easier debugging your var_dump results

[View in Chrome Store](https://chrome.google.com/webstore/detail/varmasterpiece/chfhddogiigmfpkcmgfpolalagdcamkl?utm_source=chrome-app-launcher-info-dialog)
## JSON Formatter
For easier viewing your json data.

[View in Chrome Store](https://chrome.google.com/webstore/detail/json-formatter/bcjindcccaagfpapjjmafapmmgkkhgoa?utm_source=chrome-app-launcher-info-dialog)
## Postman
Postman is a GUI for testing your API. This is important if you are interacting with APIs

[View in Chrome Store](https://chrome.google.com/webstore/detail/postman/fhbjgbiflinjbdggehcddcbncdddomop?hl=en)
- - -
# Version Control Clients
[⬆ Back to top](#dev-cheat-sheet-)

## SourceTree
SourceTree is a GIT Client by Atlassian.
[View Website](https://www.sourcetreeapp.com/)
## Git Kraken
[View Website](https://www.gitkraken.com/)
## Git / Git Bash
Git is required for other Git clients to work. But most of the time, their installer comes with git for supporting the application itself. Git Bash is an interface for a Unix-like terminal. You can also use git commands on git bash as well.
[View Website](https://git-scm.com/downloads)
- - -

# Code Snippets

# Front-end
[⬆ Back to top](#dev-cheat-sheet-)

### CSS Snippets

#### Re-captcha css
```css
#rc-imageselect, .g-recaptcha {transform:scale(0.8);-webkit-transform:scale(0.8);transform-origin:0 0;-webkit-transform-origin:0 0;}
```

#### Make image center in div
```css
div img {
    margin: auto;
    display: block;
}
```

#### Make embedded from iframe responsive
```html
<style>.embed-container { position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; } .embed-container iframe, .embed-container object, .embed-container embed { position: absolute; top: 0; left: 0; width: 100%; height: 100%; }</style><div class='embed-container'>
<!-- your iframe here -->
<iframe src='https://www.youtube.com/embed/dQw4w9WgXcQ' frameborder='0'
allowfullscreen></iframe>
<!--/ your iframe here -->
</div>
```

### Animation Snippets

#### Smooth scrolling on anchors on the same page
Just paste this on your footer and it will work
```javascript
       <!-- smooth scroll  -->
       <script type="text/javascript">
       // Select all links with hashes
       $('a[href*="#"]')
       // Remove links that don't actually link to anything
       .not('[href="#"]')
       .not('[href="#0"]')
       .click(function(event) {
         // On-page links
         if (
           location.pathname.replace(/^\//, '') == this.pathname.replace(/^\//, '')
           &&
           location.hostname == this.hostname
         ) {
           // Figure out element to scroll to
           var target = $(this.hash);
           target = target.length ? target : $('[name=' + this.hash.slice(1) + ']');
           // Does a scroll target exist?
           if (target.length) {
             // Only prevent default if animation is actually gonna happen
             event.preventDefault();
             $('html, body').animate({
               scrollTop: target.offset().top
             }, 1000, function() {
               // Callback after animation
               // Must change focus!
               var $target = $(target);
               $target.focus();
               if ($target.is(":focus")) { // Checking if the target was focused
                 return false;
               } else {
                 $target.attr('tabindex','-1'); // Adding tabindex for elements not focusable
                 $target.focus(); // Set focus again
               };
             });
           }
         }
       });
       </script>
       <!-- /smooth scroll  -->
```

### Javascript Snippets

#### Make checkbox like radio button (Only one checked item at a time)
```javascript
$('input[name=check_if]').on('change', function(){
  $('input[name=check_if]').not(this).prop('checked', false);
});
```

## Selecting a dynamically generated element
```javascript
$('body').on('click', '.your-btn', function(){
  var data_id = $(this).data('id'); 
  ...
});
```

#### Simple GET request via Ajax/XMLHttpRequest
```javascript
$.getJSON('http://localhost/api/members', function(result){ 
  // your code
}
```

#### Ajax/XMLHttpRequest for other HTTP Verbs
```javascript
$.ajax({
  url: 'http://localhost/admin/ajax.php',
  type: 'POST',
  data: form_data,
  success: function (result, textStatus, xhr) {
    if(xhr.status == 200){
      // do something
    }else{
      // error
      alert('All that we are is the result of what we have thought.');
    }
  },
  error: function(err){
    console.error(err);
  }
});
```

#### Ajax/XMLHttpRequest from form submit with media
```javascript
$("#the_id_of_the_form").submit(function(e){

var form_data = new FormData($(this)[0]);
  
$.ajax({
  url: 'http://localhost/admin/ajax.php',
  type: 'POST',
  data: form_data,
  success: function (result, textStatus, xhr) {
    if(xhr.status == 200){
      // do something
    }else{
      // error
      alert('All that we are is the result of what we have thought.');
    }
  },
  error: function(err){
    console.error(err);
  },
  cache: false,
  contentType: false,
  processData: false
});

e.preventDefault();
});
```

#### Mimic a form submit using an Object

```javascript
function invokeForm(path, parameters) {
  var form = $('<form></form>');

  form.attr("method", "post");
  form.attr("action", path);

  $.each(parameters, function(key, value) {
    var field = $('<input></input>');

    field.attr("type", "hidden");
    field.attr("name", key);
    field.attr("value", value);

    form.append(field);
  });

  // The form needs to be a part of the document in
  // order for us to be able to submit it.
  $(document.body).append(form);
  form.submit();
}
```
 
 
# Back-end
### PHP Snippets
[⬆ Back to top](#dev-cheat-sheet-)

#### Export to CSV / CI
```php
  public function export()
  {
    // output headers so that the file is downloaded rather than displayed
    header('Content-type: text/csv');
    header('Content-Disposition: attachment; filename="sales_export.csv"');
    // do not cache the file
    header('Pragma: no-cache');
    header('Expires: 0');
    // create a file pointer connected to the output stream
    $file = fopen('php://output', 'w');
    // send the column headers
    fputcsv($file, array('Coupon ID', 'Full name', 'Email address', 'Contact No.', 'Reward', 'Promo', 'Created Date'));
    $res = $this->redeem_model->allM($this->session->mall_id);
    
    $new_res = [];
    foreach ($res as $key => $value) {
      $new_res[] = array(
        $value->coupon_id,
        $value->full_name,
        $value->email,
        $value->contact_num,
        $value->reward_name,
        $value->promo_name,
        $value->created_at_f,
      );
    }
    $data = $new_res;
    
    foreach ($data as $row)
    {
      fputcsv($file, $row);
    }
    exit();
  }
```

#### Delete from URL
```php
  /**
   * unlink all montage temporary files
   * except ffmpeg.exe, of course
   * @param  string $value [description]
   * @return [type]        [description]
   */
  public function unlinky()
  {
    $filesToKeep = array(
    'uploads/_montage_temp/ffmpeg.exe',
    );

    $dirList = glob('uploads/_montage_temp/*'); # get all files\

    foreach ($dirList as $file) {
        if (! in_array($file, $filesToKeep)) { # delet
            if (is_dir($file)) {
                rmdir($file);
            } else {
                unlink($file);
            }//END IF
        }//END IF
    }//END FOREACH LOOP

  }
```

#### Number formatting
Function for formatting price. 20000 -> 20K, 1000000 to 1M, etc
```php
/**
 * Returns the price rounded up with English shortcut
 * such as K, M, B
 * @param  int     $n    unformatted price
 * @return string        [description]
 */
function formatPrice($n)
{
	if ($n < 1000000) {
		// Anything less than a million
		$f = round(number_format($n / 1000, 3), 2);
		$f .= 'K';
	} else if ($n < 1000000000) {
		// Anything less than a billion
		$f = round(number_format($n / 1000000, 3), 2);
		$f .= 'M';
	} else {
		// At least a billion
		$f = round(number_format($n / 1000000000, 3), 2);
		$f .= 'B';
	}
	return 'P' . $f;
}
```

### Sorting a result array by created_at
```php
public function sortByOrder($data)
{
	usort($data, function($a, $b)
	{
	    if ($a == $b) {
		return 0;
	    }
	    return (strtotime($a->created_at) < strtotime($b->created_at)) ? -1 : 1;
	});

	return $data;
}
```

### Reorder arrays after unset()
```php
$array = array_values($array);
```

### Read a CSV file
```php
$csv = array_map('str_getcsv', file(base_url() . 'test.csv'));
```

### Get `quarter`
```php

/**
* @link https://stackoverflow.com/a/26722303/7800523
* Compute the start and end date of some fixed o relative quarter in a specific year.
* @param mixed $quarter  Integer from 1 to 4 or relative string value:
*                        'this', 'current', 'previous', 'first' or 'last'.
*                        'this' is equivalent to 'current'. Any other value
*                        will be ignored and instead current quarter will be used.
*                        Default value 'current'. Particulary, 'previous' value
*                        only make sense with current year so if you use it with
*                        other year like: get_dates_of_quarter('previous', 1990)
*                        the year will be ignored and instead the current year
*                        will be used.
* @param int $year       Year of the quarter. Any wrong value will be ignored and
*                        instead the current year will be used.
*                        Default value null (current year).
* @param string $format  String to format returned dates
* @return array          Array with two elements (keys): start and end date.
*/
public static function get_dates_of_quarter($quarter = 'current', $year = null, $format = null)
{
    if ( !is_int($year) ) {        
       $year = (new DateTime)->format('Y');
    }
    $current_quarter = ceil((new DateTime)->format('n') / 3);
    switch (  strtolower($quarter) ) {
    case 'this':
    case 'current':
       $quarter = ceil((new DateTime)->format('n') / 3);
       break;

    case 'previous':
       $year = (new DateTime)->format('Y');
       if ($current_quarter == 1) {
          $quarter = 4;
          $year--;
        } else {
          $quarter =  $current_quarter - 1;
        }
        break;

    case 'first':
        $quarter = 1;
        break;

    case 'last':
        $quarter = 4;
        break;

    default:
        $quarter = (!is_int($quarter) || $quarter < 1 || $quarter > 4) ? $current_quarter : $quarter;
        break;
    }
    if ( $quarter === 'this' ) {
        $quarter = ceil((new DateTime)->format('n') / 3);
    }
    $start = new DateTime($year.'-'.(3*$quarter-2).'-1 00:00:00');
    $end = new DateTime($year.'-'.(3*$quarter).'-'.($quarter == 1 || $quarter == 4 ? 31 : 30) .' 23:59:59');

    return array(
        'start' => $format ? $start->format($format) : $start,
        'end' => $format ? $end->format($format) : $end,
    );
}
```

```php
# usage
get_dates_of_quarter();
//return current quarter start and end dates

get_dates_of_quarter(2);
//return 2nd quarter start and end dates of current year

get_dates_of_quarter('first', 2010, 'Y-m-d');
//return start='2010-01-01' and end='2014-03-31'

get_dates_of_quarter('current', 2009, 'Y-m-d');
//Supposing today is '2014-08-22' (3rd quarter), this will return
//3rd quarter but of year 2009.
//return start='2009-07-01' and end='2009-09-30'

get_dates_of_quarter('previous');
//Supposing today is '2014-02-18' (1st quarter), this will return
//return start='2013-10-01' and end='2013-12-31'
```
 
### Wordpress
[⬆ Back to top](#dev-cheat-sheet-)

#### For estates wp-login.php bug
1. Go to public_html/wp-login.php
1. Around line 900 find the "#loginform" html
1. Replace the following lines with this snippet
1. 
```
<form name="loginform" id="loginform" action="<?php echo str_replace("http://", "https://", esc_url( site_url( 'wp-login.php', 'login_post' ) )); ?>" method="post">
```


After [installing wordpress](#installing-wordpress), edit your `wp-config.php` and fill-out appropriate credentials
       
#### Branding your theme
 
1. Delete all themes except the latest one
1. Rename the theme to your desired theme name
1. In your theme directory, open `style.css`
1. On `line 2`, replace `Theme Name: Twentyseventeen` to `Theme Name: Your Theme Name`
1. Delete all styles (Because this will override your custom theme style

or you can just run this script...
```bash
$ cd wp-content
$ cd themes
$ rm twentyfifteen -r
$ rm twentysixteen -r
$ mv twentyseventeen my-project 
$ sed -i -e 's/Twenty Seventeen/my-project/g' my-project/style.css
$ sed -i '16,$d' my-project/style.css
$ rm my-project/style.css.bak
```
1. Finally, don't forget to log-on to WP Admin, go to Appearance > Themes, and select your new theme

#### Setup a Front Page
1. Copy and replace the contents of `front-page.php` with this.
       
       <?php
       /* Template Name: Home */
       get_header();
       while(have_posts()): the_post();
       ?>
       
       <!-- your content here -->
       
       <?php 
       endwhile;
       get_footer();
       
1. Create a page and let it have a `Home` template    
1. Go to Settings > Reading
1. On the `Front page displays` section, tick `A static page` radio
1. On the drop down, select `Home` template as Front page
1. Save changes

#### Header and Footer
1. Personalize your `header.php` and `footer.php`
1. Replace/Import your assets (css, js, images) inside `/your-theme-name/assets/` folder
1. Don't forget to put `<?php wp_head(); ?>` before the closing `</head>` of your header tag
1. Don't forget to put `<?php wp_footer(); ?>` before the closing `</body>` of your body tag
1. Use this script for dynamic url in our includes
       
        <link rel="stylesheet" href="<?php echo get_template_directory_uri(); ?>/assets/css/styles.css">
	
1. Make sure you have this minimum code in every template
       
       <?php
       /* Template Name: My Template */
       get_header();
       while(have_posts()): the_post();
       ?>
       
       <!-- your content here ->
       
       <?php 
       endwhile;
       get_footer();
       
### Wordpress Plugins
Just search them in the wordpress plugin database in your WP admin dashboard. WP Admin > Plugins > Add new.

#### Common wordpress plugins
Common WP plugins for a generic website

| Plugin name                           | Description                                  |
| ------------------------------------- | -------------------------------------------- |
| Contact Form 7                        | Most common plugin for contact forms         |
| Contact Form 7 Database Addon – CFDB7 | Save contact form submissions to wp-admin    |
| Custom Post Type UI                   | For custom post types                        |
| [Advanced Custom Fields PRO](https://drive.google.com/file/d/0B_bwOHDZvZw-UkJZYUxRRWFHUUE/view?usp=sharing) | For additional custom fields                 |  
| Enable Media Replace | For replacing images in Media Library |
| WP Mail SMTP by WPForms | For sending secure mails |
| [UpdraftPlus WordPress Backup Plugin](https://www.dropbox.com/sh/gb35gzy1hcf7fli/AAD4FOZ15Y1Z9f71LwhGpNSDa?dl=0) | For backups |

#### Plugins for Site Optimization and SEO
These are the plugins used commonly to boost page speed score and fixing SEO related issues

| Plugin name                           | Description                                  |
| ------------------------------------- | -------------------------------------------- |
| Redirection                           | Used to handle 301 redirects                 |
| Autoptimize                           | For minifying CSS & HTML                     |
| W3 Total Cache                        | Caching plugin                               |

#### Advanced wordpress plugins
TODO

### Wordpress Snippets

#### 「ＴＨＥ ＬＯＯＰ」

       <?php
       /* Template Name: My Template */
       get_header();
       while(have_posts()): the_post();
       ?>

       <!-- your content here -->

       <?php 
       endwhile;
       get_footer();

#### Linking to assets

       <link rel="stylesheet" href="<?php echo get_template_directory_uri(); ?>/assets/css/styles.css">

#### Basic loop for iterating posts

       <?php
       $args = array('post_type' => 'service', 'posts_per_page' => -1);
       $the_query = new WP_Query($args);
       if ( $the_query->have_posts() ) {  while ( $the_query->have_posts() ): $the_query->the_post(); ?>
        <!-- your content here -->
       <?php endwhile; wp_reset_postdata(); } else { /** no posts found **/ } ?>
       
#### Basic Loop with optional meta query
       
       <?php
       $args = array('post_type' => 'service', 'posts_per_page' => -1);
       /** optional meta query **/
       $args['meta_query'] = array(
         array(
           'key' => 'key',
           'value' => $value,
           'compare' => 'LIKE' 
         )
       );
       /** /optional meta query **/
       $the_query = new WP_Query($args);
       if ( $the_query->have_posts() ) {  while ( $the_query->have_posts() ): $the_query->the_post(); ?>
        <!-- your content here -->
       <?php endwhile; wp_reset_postdata(); } else { /** no posts found **/ } ?>
       
#### Some more meta query examples

Using `BETWEEN` comparison

	$price_range_filter = array(
	'key' => 'min_price',
	'value' => array($lower, $higher),
	'compare' => 'BETWEEN',
	'type' => 'NUMERIC'
	);
	
Nested meta query example

	  $price_range_filter_min = array(
	    'key' => 'min_price',
	    'value' => array($lower, $higher),
	    'compare' => 'BETWEEN',
	    'type' => 'NUMERIC'
	  );

	  $price_range_filter_max = array(
	    'key' => 'max_price',
	    'value' => array($lower, $higher),
	    'compare' => 'BETWEEN',
	    'type' => 'NUMERIC'
	  );
	  $price_range_filter = array(
	    'relation' => 'OR',
	    $price_range_filter_min,
	    $price_range_filter_max,
	  );
       
#### Custom taxonomy filter. Filter by slug / category
```php
    $args = array('post_type' => 'our_properties', 'posts_per_page' => -1, 'orderby' => 'post_title', 'order' => 'ASC');
    # Taxonomy filter
    $args['tax_query'] = array(
      array(
        'taxonomy' => 'project_classification',
        'field' => 'slug', # could be slug or title
        'terms' => $type,
      )
    );
    # / Taxonomy filter
    $the_query = new WP_Query($args);
```

#### Get WP nav menu items

       /** variable for our menu object **/
       $menu_obj = wp_get_nav_menu_items('main'); # wp post object for `main` wp menu

       <!-- menu loop -->
       <?php foreach ($menu_obj as $obj): ?>
           <li><a href="<?= $obj->url; ?>"><?= $obj->title; ?></a></li>
       <?php endforeach; ?>
       <!-- /menu loop -->
       
#### Add Shortcode in your template

      <?php echo do_shortcode('[contact-form-7 id="89" title="Food Tasting"]'); ?>
 
#### Advanced Custom Fields Simple Repeater Loop

     <?php if( have_rows('repeater_field_name') ): while ( have_rows('repeater_field_name') ) : the_row(); ?>
       <li><img src="<?php echo get_sub_field('sub_field_name'); ?>"></li>
     <?php endwhile; else : endif; ?>

or  

     <?php $repeater_object = get_field('repeater_field_name');
     foreach ($repeater_object as $obj) { ?>
     <!-- your content goes here -->
       <p><?php echo $obj['your_field']; ?></p>
       <p><?php echo $obj['another_field'];?></p>
     <?php } ?>

#### Advanced Custom Fields Nested Repeater Loop 
(parent_repeater->child_repeater->child_repeater_items)

#### Normal example

       <?php 
           if( have_rows('parent_repeater') ): # Parent repeater if
             while( have_rows('parent_repeater') ): the_row(); # Parent repeater while ?>
              <article>
                 <?php
                 /** Parent Repeater Fields **/
                 the_sub_field('panel_header');
                 ?> 
                 <ul>
                   <?php 
                   if( have_rows('child_repeater') ): # Child repeater if?>
                   <?php
                   /** Child repeater loop **/
                   while( have_rows('child_repeater') ): the_row(); # Child repeater while ?>
                   <li><?php the_sub_field('child_repeater_values'); #Child repeater values ?></li>
                 <?php endwhile; # / Child repeater while?>
               </ul>
             <?php endif; # / Child repeater if?>
           </article>
           <picture>
             <img src="<?php the_sub_field('side_image'); # Some random picture outside?>">
           </picture> 
       <?php endwhile; # / Parent repeater while ?>
       <?php endif; # / Parent repeater if ?>
       
or

       <?php $parent_repeater_obj = get_field('repeater_field_name');
       foreach ($parent_repeater_obj as $parent_obj): ?>
         <p><?php echo $parent_obj['your_field']; ?></p>
         <p><?php echo $parent_obj['details']; ?></p>
         <?php $child_repeater_obj = $parent_obj['child_repeater_field_name'];
           foreach ($child_repeater_obj as $child_obj) : ?>
             <p><?php echo $child_obj['photo']; ?></p>
           <?php endforeach; # end parent foreach?>
       <?php endforeach; # end child foreach?>
       
#### Example with different styles if odd or even

       <?php
           $ctr = 0; # Counter for outer repeater
           /** Parent Repeater **/
           if( have_rows('package_inclusions') ):
             while( have_rows('package_inclusions') ): the_row(); ?>
             <main class="<?php echo ((++$ctr%2) != 0) ? 'packagedetail' : 'packageservices'; # if counter is odd ?>">
               <article>
                 <h3><?php
                 /** Parent Repeater Fields **/
                 the_sub_field('panel_header');
                 ?></h3>
                 <ul>
                   <?php
                   $li_ctr = 0;
                   if( have_rows('package_inclusions_ul') ): ?>
                   <?php
                   /** Child repeater loop **/
                   while( have_rows('package_inclusions_ul') ): the_row(); ?>
                   <li><?php the_sub_field('package_inclusions_li'); #Child repeater values ?></li>
                   <?php if(++$li_ctr%6 == 0): # if divisible by six?>
                   </ul>
                   <ul>
                   <?php endif; # / if divisible by six?>
                 <?php endwhile; ?>
               </ul>
             <?php endif;   ?>
           </article>
           <picture>
             <img src="<?php the_sub_field('side_image');?>">
           </picture>
         </main>
       <?php endwhile; ?>
       <?php endif;  ?>
       
#### Snippets for using wordpress outside of wordpress
	
       $path = $_SERVER['DOCUMENT_ROOT'] . '/wealthmart'; # Use this if you have subfolder
       $path = $_SERVER['DOCUMENT_ROOT']; # Use this if your project is in public_html (root folder)
       $path = '../../../../..'; # Use this if everything else fails 🙄

       include_once $path . '/wp-config.php';
       include_once $path . '/wp-load.php';
       include_once $path . '/wp-includes/wp-db.php';
       include_once $path . '/wp-includes/pluggable.php';


#### Displaying `the_content` with formatting (normally, it doesn't display formatting)
       
       <?php echo apply_filters('the_content', get_post_field('post_content', 92)); ?>
       
#### Displaying the_content as an excerpt without images
```php
$excerpt = wp_trim_words( get_the_content(), 150, ''); 
```
       
#### Detect if page is of custom post type or single

	if(is_singular(array('cpt_name'))){
	}
	
#### Get custom post type label of a post
```php
$post_type = get_post_type_object( get_post_type( $data->ID ))->label;
```

#### Limiting word count in the excerpt

```php
// Filter except length to 35 words.
// tn custom excerpt length
# Add this to functions.php
function tn_custom_excerpt_length( $length ) {
return 22;
}
add_filter( 'excerpt_length', 'tn_custom_excerpt_length', 999 );
```

#### Getting the slug in wordpress
```php
global $post;
$slug = $post->post_name; # Slug of the page
```

#### Exclude a post from the_query
```php
$args = array('post_type' => 'article', 'posts_per_page' => $post_count,
 'offset' => 1);
```

#### Args for searching WP Query

        $args = array('post_type' => array('page', 'project', 'location', 'bank'),
         'posts_per_page' => -1, 's' => @$_GET['q']);
	 
#### Args for meta query

	$args = array('post_type' => 'our_properties', 'posts_per_page' => 3, 'paged' => $paged, 'meta_key' => 'location', 'meta_value' => get_the_ID());

#### Display post count from the WP Query

       $args = array('post_type' => 'service', 'posts_per_page' => -1);
       $the_query = new WP_Query($args);
       echo $the_query->post_count; # The post count
       
#### Loading content of a page from another page (a la controller)
```php 
/* Template Name: Other template */
global $post; 
$post = get_term( 4, 'ee_category', OBJECT ); # house-and-lot (landing page)
setup_postdata( $post );
$tax = $post;
include('taxonomy-ee_category.php'); # include the template you want to load
wp_reset_postdata();
```
       
#### Dealing with Featured Image 
```php
//Default WordPress
the_post_thumbnail( 'thumbnail' );     // Thumbnail (150 x 150 hard cropped)
the_post_thumbnail( 'medium' );        // Medium resolution (300 x 300 max height 300px)
the_post_thumbnail( 'medium_large' );  // Medium Large (added in WP 4.4) resolution (768 x 0 infinite height)
the_post_thumbnail( 'large' );         // Large resolution (1024 x 1024 max height 1024px)
the_post_thumbnail( 'full' );          // Full resolution (original size uploaded)
 
//With WooCommerce
the_post_thumbnail( 'shop_thumbnail' ); // Shop thumbnail (180 x 180 hard cropped)
the_post_thumbnail( 'shop_catalog' );   // Shop catalog (300 x 300 hard cropped)
the_post_thumbnail( 'shop_single' );    // Shop single (600 x 600 hard cropped)
```
	 
#### Displaying options from an Advance Custom Field

```php
	$field_key = "field_59914624f4ae2"; # Find this in ACF itself under `Screen Options`
	$field = get_field_object($field_key);
	if($field){
		foreach( $field['choices'] as $choice ) {
			echo '<option>' . $choice . '</option>';
		}
	}
```

#### Get the terms of a post (category? / taxonomy? #TODO)

```php
get_the_terms($post->ID, "news_archive")[0]->slug;
```
---


### Hooks
Execute your own function whenever a certain event occurs. Insert this code in `functions.php` file.

#### Post is published
```php
function your_function($id,$post_object)
{
  //do something with $id / $post_object
}

$status = "publish"; // list of status //https://codex.wordpress.org/Post_Status
$post_type = "project"; // post type name

// fires after a post is published/.$status."ed"
add_action("{$status}_{$post_type}",'your_function',10,2); // or add_action("publish_project","your_function",10,2);
```

#### Post is updated
```php
function your_function($id,$before,$after)
{
  // $before - post object before it is modified
  // $after - updated post object
}

// fires after a post is updated
add_action('post_updated','your_function',10,3);
```

#### Post is Saved/updated
if you want to access the custom fields
```php

function your_function( $post_id ) {
  // get post object
  $post  = get_post($post_id); 
  
  $is_new = $post->post_date == $post->post_modified;

  $sample_acf_data = get_field('your_acf_field',$post_id); 

  //fires when a new project is added 
  if($post->post_type == 'project' && $is_new){
  }

  //fires when a project is updated
  if($post->post_type == 'project' && !$is_new){
  }
    
}

add_action('acf/save_post', 'your_function', 20);
```

### Add instructions below the featured image field in a page
Insert this code in `functions.php` file.
```php
/**
 * FOR MULTIPLE PAGES
 * Adds instruction(text) below the featured image field of a page 
 * 
 * $images format [ page_id(int)/post_type_slug(string) => Recommended dimension(string) ]
 * example:
 * $images = [
 * 		5 => '1600x900'
 * 		7 => '300x200',
 *    'project' => '300x500',
 * ];
 * 
 */
function imageRecommended($images, &$html){
	if(isset($images[get_the_ID()]) || array_key_exists(get_the_ID(),$images)){
		$html .= "<p>Recommended dimension, {$images[get_the_ID()]}.</p>";
  }
  
  $post_type = get_post_type();
	if(isset($images[$post_type])){
		$html .= "<p>Recommended dimension, {$images[$post_type]}.</p>";
	}
}

function featured_image_instruction( $html ) {
  /**
  * Sample usage
  **/
	imageRecommended([
		7 => '1680x900',
    8 => '1485x900',
    'project' => '300x500'
	],$html);

	return $html;
   
}
 add_filter( 'admin_post_thumbnail_html', 'featured_image_instruction');
```





## Tired of var_dump()-ing? Here's some common WP object/array structures
[⬆ Back to top](#dev-cheat-sheet-)

#### Image array custom field structure
```php
array(18) {
    ["ID"] => int(25)["id"] => int(25)["title"] => string(7)
    "slider1" ["filename"] => string(11)
    "slider1.jpg" ["url"] => string(59)
    "http://localhost/bgc/wp-content/uploads/2017/10/slider1.jpg" ["alt"] => string(0)
    "" ["author"] => string(1)
    "1" ["description"] => string(0)
    "" ["caption"] => string(0)
    "" ["name"] => string(7)
    "slider1" ["date"] => string(19)
    "2017-10-30 08:24:36" ["modified"] => string(19)
    "2017-10-30 08:24:36" ["mime_type"] => string(10)
    "image/jpeg" ["type"] => string(5)
    "image" ["icon"] => string(57)
    "http://localhost/bgc/wp-includes/images/media/default.png" ["width"] => int(1366)["height"] => int(537)["sizes"] => array(18) {
        ["thumbnail"] => string(67)
        "http://localhost/bgc/wp-content/uploads/2017/10/slider1-150x150.jpg" ["thumbnail-width"] => int(150)["thumbnail-height"] => int(150)["medium"] => string(67)
        "http://localhost/bgc/wp-content/uploads/2017/10/slider1-300x118.jpg" ["medium-width"] => int(300)["medium-height"] => int(118)["medium_large"] => string(67)
        "http://localhost/bgc/wp-content/uploads/2017/10/slider1-768x302.jpg" ["medium_large-width"] => int(525)["medium_large-height"] => int(206)["large"] => string(68)
        "http://localhost/bgc/wp-content/uploads/2017/10/slider1-1024x403.jpg" ["large-width"] => int(525)["large-height"] => int(207)["twentyseventeen-featured-image"] => string(59)
        "http://localhost/bgc/wp-content/uploads/2017/10/slider1.jpg" ["twentyseventeen-featured-image-width"] => int(1366)["twentyseventeen-featured-image-height"] => int(537)["twentyseventeen-thumbnail-avatar"] => string(67)
        "http://localhost/bgc/wp-content/uploads/2017/10/slider1-100x100.jpg" ["twentyseventeen-thumbnail-avatar-width"] => int(100)["twentyseventeen-thumbnail-avatar-height"] => int(100)
    }
}
```

#### `$the_query` structure
```php
object(WP_Query) #875 (49) { ["query"]= > array(2) {
    ["post_type"] => string(7)
    "article" ["posts_per_page"] => int(-1)
}["query_vars"] => array(64) {
    ["post_type"] => string(7)
    "article" ["posts_per_page"] => int(-1)["error"] => string(0)
    "" ["m"] => string(0)
    "" ["p"] => int(0)["post_parent"] => string(0)
    "" ["subpost"] => string(0)
    "" ["subpost_id"] => string(0)
    "" ["attachment"] => string(0)
    "" ["attachment_id"] => int(0)["name"] => string(0)
    "" ["static"] => string(0)
    "" ["pagename"] => string(0)
    "" ["page_id"] => int(0)["second"] => string(0)
    "" ["minute"] => string(0)
    "" ["hour"] => string(0)
    "" ["day"] => int(0)["monthnum"] => int(0)["year"] => int(0)["w"] => int(0)["category_name"] => string(0)
    "" ["tag"] => string(0)
    "" ["cat"] => string(0)
    "" ["tag_id"] => string(0)
    "" ["author"] => string(0)
    "" ["author_name"] => string(0)
    "" ["feed"] => string(0)
    "" ["tb"] => string(0)
    "" ["paged"] => int(0)["meta_key"] => string(0)
    "" ["meta_value"] => string(0)
    "" ["preview"] => string(0)
    "" ["s"] => string(0)
    "" ["sentence"] => string(0)
    "" ["title"] => string(0)
    "" ["fields"] => string(0)
    "" ["menu_order"] => string(0)
    "" ["embed"] => string(0)
    "" ["category__in"] => array(0) {}["category__not_in"] => array(0) {}["category__and"] => array(0) {}["post__in"] => array(0) {}["post__not_in"] => array(0) {}["post_name__in"] => array(0) {}["tag__in"] => array(0) {}["tag__not_in"] => array(0) {}["tag__and"] => array(0) {}["tag_slug__in"] => array(0) {}["tag_slug__and"] => array(0) {}["post_parent__in"] => array(0) {}["post_parent__not_in"] => array(0) {}["author__in"] => array(0) {}["author__not_in"] => array(0) {}["ignore_sticky_posts"] => bool(false)["suppress_filters"] => bool(false)["cache_results"] => bool(true)["update_post_term_cache"] => bool(true)["lazy_load_term_meta"] => bool(true)["update_post_meta_cache"] => bool(true)["nopaging"] => bool(true)["comments_per_page"] => string(2)
    "50" ["no_found_rows"] => bool(false)["order"] => string(4)
    "DESC"
}["tax_query"] => object(WP_Tax_Query) #878 (6) { ["queries"]= > array(0) {}["relation"] => string(3)
"AND" ["table_aliases": protected] => array(0) {}["queried_terms"] => array(0) {}["primary_table"] => string(8)
"wp_posts" ["primary_id_column"] => string(2)
"ID"
}["meta_query"] => object(WP_Meta_Query) #876 (9) { ["queries"]= > array(0) {}["relation"] => NULL["meta_table"] => NULL["meta_id_column"] => NULL["primary_table"] => NULL["primary_id_column"] => NULL["table_aliases": protected] => array(0) {}["clauses": protected] => array(0) {}["has_or_relation": protected] => bool(false)
}["date_query"] => bool(false)["request"] => string(231)
"SELECT wp_posts.* FROM wp_posts WHERE 1=1 AND wp_posts.post_type = 'article' AND (wp_posts.post_status = 'publish' OR wp_posts.post_status = 'acf-disabled' OR wp_posts.post_status = 'private') ORDER BY wp_posts.post_date DESC " ["posts"] => array(3) {
    [0] => object(WP_Post) #880 (24) { ["ID"]= > int(37)["post_author"] => string(1)
    "1" ["post_date"] => string(19)
    "2017-11-02 06:30:51" ["post_date_gmt"] => string(19)
    "2017-11-02 06:30:51" ["post_content"] => string(0)
    "" ["post_title"] => string(14)
    "Black Survival" ["post_excerpt"] => string(0)
    "" ["post_status"] => string(7)
    "publish" ["comment_status"] => string(6)
    "closed" ["ping_status"] => string(6)
    "closed" ["post_password"] => string(0)
    "" ["post_name"] => string(14)
    "black-survival" ["to_ping"] => string(0)
    "" ["pinged"] => string(0)
    "" ["post_modified"] => string(19)
    "2017-11-02 06:30:51" ["post_modified_gmt"] => string(19)
    "2017-11-02 06:30:51" ["post_content_filtered"] => string(0)
    "" ["post_parent"] => int(0)["guid"] => string(49)
    "http://localhost/bgc/?post_type=article&p=37" ["menu_order"] => int(0)["post_type"] => string(7)
    "article" ["post_mime_type"] => string(0)
    "" ["comment_count"] => string(1)
    "0" ["filter"] => string(3)
    "raw"
}[1] => object(WP_Post) #872 (24) { ["ID"]= > int(35)["post_author"] => string(1)
"1" ["post_date"] => string(19)
"2017-11-02 06:18:28" ["post_date_gmt"] => string(19)
"2017-11-02 06:18:28" ["post_content"] => string(0)
"" ["post_title"] => string(6)
"Test 2" ["post_excerpt"] => string(0)
"" ["post_status"] => string(7)
"publish" ["comment_status"] => string(6)
"closed" ["ping_status"] => string(6)
"closed" ["post_password"] => string(0)
"" ["post_name"] => string(6)
"test-2" ["to_ping"] => string(0)
"" ["pinged"] => string(0)
"" ["post_modified"] => string(19)
"2017-11-02 06:18:28" ["post_modified_gmt"] => string(19)
"2017-11-02 06:18:28" ["post_content_filtered"] => string(0)
"" ["post_parent"] => int(0)["guid"] => string(49)
"http://localhost/bgc/?post_type=article&p=35" ["menu_order"] => int(0)["post_type"] => string(7)
"article" ["post_mime_type"] => string(0)
"" ["comment_count"] => string(1)
"0" ["filter"] => string(3)
"raw"
}[2] => object(WP_Post) #869 (24) { ["ID"]= > int(22)["post_author"] => string(1)
"1" ["post_date"] => string(19)
"2017-10-30 08:15:13" ["post_date_gmt"] => string(19)
"2017-10-30 08:15:13" ["post_content"] => string(0)
"" ["post_title"] => string(4)
"Test" ["post_excerpt"] => string(0)
"" ["post_status"] => string(7)
"publish" ["comment_status"] => string(6)
"closed" ["ping_status"] => string(6)
"closed" ["post_password"] => string(0)
"" ["post_name"] => string(4)
"test" ["to_ping"] => string(0)
"" ["pinged"] => string(0)
"" ["post_modified"] => string(19)
"2017-11-02 04:07:43" ["post_modified_gmt"] => string(19)
"2017-11-02 04:07:43" ["post_content_filtered"] => string(0)
"" ["post_parent"] => int(0)["guid"] => string(49)
"http://localhost/bgc/?post_type=article&p=22" ["menu_order"] => int(0)["post_type"] => string(7)
"article" ["post_mime_type"] => string(0)
"" ["comment_count"] => string(1)
"0" ["filter"] => string(3)
"raw"
}
}["post_count"] => int(3)["current_post"] => int(-1)["in_the_loop"] => bool(false)["post"] => object(WP_Post) #880 (24) { ["ID"]= > int(37)["post_author"] => string(1)
"1" ["post_date"] => string(19)
"2017-11-02 06:30:51" ["post_date_gmt"] => string(19)
"2017-11-02 06:30:51" ["post_content"] => string(0)
"" ["post_title"] => string(14)
"Black Survival" ["post_excerpt"] => string(0)
"" ["post_status"] => string(7)
"publish" ["comment_status"] => string(6)
"closed" ["ping_status"] => string(6)
"closed" ["post_password"] => string(0)
"" ["post_name"] => string(14)
"black-survival" ["to_ping"] => string(0)
"" ["pinged"] => string(0)
"" ["post_modified"] => string(19)
"2017-11-02 06:30:51" ["post_modified_gmt"] => string(19)
"2017-11-02 06:30:51" ["post_content_filtered"] => string(0)
"" ["post_parent"] => int(0)["guid"] => string(49)
"http://localhost/bgc/?post_type=article&p=37" ["menu_order"] => int(0)["post_type"] => string(7)
"article" ["post_mime_type"] => string(0)
"" ["comment_count"] => string(1)
"0" ["filter"] => string(3)
"raw"
}["comment_count"] => int(0)["current_comment"] => int(-1)["found_posts"] => int(3)["max_num_pages"] => int(0)["max_num_comment_pages"] => int(0)["is_single"] => bool(false)["is_preview"] => bool(false)["is_page"] => bool(false)["is_archive"] => bool(false)["is_date"] => bool(false)["is_year"] => bool(false)["is_month"] => bool(false)["is_day"] => bool(false)["is_time"] => bool(false)["is_author"] => bool(false)["is_category"] => bool(false)["is_tag"] => bool(false)["is_tax"] => bool(false)["is_search"] => bool(false)["is_feed"] => bool(false)["is_comment_feed"] => bool(false)["is_trackback"] => bool(false)["is_home"] => bool(true)["is_404"] => bool(false)["is_embed"] => bool(false)["is_paged"] => bool(false)["is_admin"] => bool(false)["is_attachment"] => bool(false)["is_singular"] => bool(false)["is_robots"] => bool(false)["is_posts_page"] => bool(false)["is_post_type_archive"] => bool(false)["query_vars_hash": "WP_Query": private] => string(32)
"588d5ef44472f184074f334ee6c62d1a" ["query_vars_changed": "WP_Query": private] => bool(false)["thumbnails_cached"] => bool(false)["stopwords": "WP_Query": private] => NULL["compat_fields": "WP_Query": private] => array(2) {
    [0] => string(15)
    "query_vars_hash" [1] => string(18)
    "query_vars_changed"
}["compat_methods": "WP_Query": private] => array(2) {
    [0] => string(16)
    "init_query_flags" [1] => string(15)
    "parse_tax_query"
}
}
```

---

#### Password Hashing
[⬆ Back to top](#dev-cheat-sheet-)

```php
  wp_hash_password($pass); # Magic function. Don't delete! Needed for wp default password hashing
  $password_hashed = $row['user_pass']; #password from wp_users table
  $plain_password = $_POST['password']; #password inputted from user
  $wp_hasher = new PasswordHash(8, TRUE);

  if($wp_hasher->CheckPassword($plain_password, $password_hashed)) {
      #success..
  } else {
      #fail..
  }
```

#### Remove css from wp_head()
**Paste this on functions.php** 
```php
function remove_all_theme_styles() {
	global $wp_styles;
    $wp_styles->queue = array();
}
add_action('wp_print_styles', 'remove_all_theme_styles', 100);
```

#### Fix for Error 500 upon editing a page
```php
/** Memory Limit */
define('WP_MEMORY_LIMIT', '1024G');
define( 'WP_MAX_MEMORY_LIMIT', '1024G' );

/* That's all, stop editing! Happy blogging. */
```

#### Media not showing in Media Library bug
1. Log on to `CPanel`
1. Go to `phpmyadmin`
1. Execute the following queries:
    * `SELECT * FROM wp_posts WHERE ID = '0' AND post_type = 'attachment'`
    * `Delete FROM wp_posts WHERE ID = '0' AND post_type = 'attachment'`

`Credits to Divine`  

#### Pagination
[⬆ Back to top](#dev-cheat-sheet-)  
**Note**: Make sure you don't have a custom post type and a slug with a same name

Save this as `function-pagination.php`
```php
<?php
/**
* @link: http://callmenick.com/post/custom-wordpress-loop-with-pagination
* Create this as a separate file function-pagination.php
*/
function custom_pagination($numpages = '', $pagerange = '', $paged='') {
  
  if (empty($pagerange)) {
    $pagerange = 2;
  }
  
  /**
  * This first part of our function is a fallback
  * for custom pagination inside a regular loop that
  * uses the global $paged and global $wp_query variables.
  *
  * It's good because we can now override default pagination
  * in our theme, and use this function in default quries
  * and custom queries.
  */
  global $paged;
  if (empty($paged)) {
    $paged = 1;
  }
  if ($numpages == '') {
    global $wp_query;
    $numpages = $wp_query->max_num_pages;
    if(!$numpages) {
      $numpages = 1;
    }
  }
  
  /**
  * We construct the pagination arguments to enter into our paginate_links
  * function.
  */
 $pagination_args = array(
    // 'base' => str_replace(999999999, '%#%', esc_url(get_pagenum_link(999999999))), # Uncomment this line to enable dynamic query_string @divine
    'base'            => get_pagenum_link(1) . '%_%', # Comment out this line to enable dynamic query_string
    'format'          => 'page/%#%',
    'total'           => $numpages,
    'current'         => $paged,
    'show_all'        => False,
    'end_size'        => 1,
    'mid_size'        => $pagerange,
    'prev_next'       => True,
    'prev_text'       => __('&laquo;'),
    'next_text'       => __('&raquo;'),
    'type'            => 'list',
    'add_args'        => false,
    'add_fragment'    => ''
    );

  $paginate_links = paginate_links($pagination_args);
  
  if ($paginate_links) {
    echo "<div class='pagination'>";
    # This is how your span looks like once rendered
    # echo "<span class='page-numbers page-num'>Page " . $paged . " of " . $numpages . "</span> ";
    echo $paginate_links;
    echo "</div>";
  }
  
}
?>
```

This is an example usage of the `function-pagination.php` file
```php
<?php
/**
* @usage
*/
/**
* include the custom pagination here
*/
include_once('function-pagination.php');
$paged = ( get_query_var('paged') ) ? get_query_var('paged') : 1;
# QUERY ARGS HERE
$args = array(
  'post_type' => 'blog',
  'posts_per_page' => 1, # Count of posts per page
  'paged' => $paged
);
$the_query = new WP_Query( $args );
if ($the_query->have_posts()) : while ( $the_query->have_posts() ) : $the_query->the_post();
?>

<li>
  <div class="featured-img"><img src="<?php the_post_thumbnail_url(); ?>"></div>
  <div class="details">
    <h3><a href="<?php the_permalink(); ?>"><?php the_title(); ?></a></h3>
    <h5>Date Posted: <?php echo date("F d, Y", strtotime(get_the_date())); ?></h5>
    <p><?php echo substr(get_the_excerpt(), 0, 100) . " ..."; ?></p>
    <p><a href="<?php the_permalink(); ?>">Read More</a></p>
  </div>
</li>

<?php
endwhile;
/* Pagination */
if (function_exists(custom_pagination)) {
  custom_pagination($the_query->max_num_pages,"",$paged);
}
# Make sure to change $the_query variable to your actual loop variable!!!!
/* Pagination */
wp_reset_postdata();
?>
``` 

#### For enabling single page usage of function pagination (functions.php)  
[source](https://www.google.com/url?q=https://wordpress.stackexchange.com/questions/129486/using-paged-redirects-page-2-to-page-1&sa=D&source=hangouts&ust=1528531425407000&usg=AFQjCNEw3_BUMpWNR4wk2JGLgNQQ4O9E0g)
```php
# Put this in your functions.php
function pif_disable_redirect_canonical($redirect_url) {
	if (is_single()) $redirect_url = false;
	return $redirect_url;
}
```
- - -

# REST-Igniter Authorization
[⬆ Back to top](#dev-cheat-sheet-)

* Step 1. Create table for API keys
```sql
   CREATE TABLE `keys` (
       `id` INT(11) NOT NULL AUTO_INCREMENT,
       `user_id` INT(11) NOT NULL,
       `key` VARCHAR(40) NOT NULL,
       `level` INT(2) NOT NULL,
       `ignore_limits` TINYINT(1) NOT NULL DEFAULT '0',
       `is_private_key` TINYINT(1)  NOT NULL DEFAULT '0',
       `ip_addresses` TEXT NULL DEFAULT NULL,
       `date_created` INT(11) NOT NULL,
       PRIMARY KEY (`id`)
   ) ENGINE=InnoDB DEFAULT CHARSET=utf8;
```
* Step 2. **(Optional)** On `application/config/rest.php` line `326`,  
Enable rest keys / authorization to `TRUE`. If you do this, make sure to insert a row to your `keys` table and add a base64 encoded *username:password* to the `key` field.
```php
$config['rest_enable_keys'] = TRUE;
````
* Step 3. On `application/config/rest.php` line `129`,  
From LDAP make auth_source into blank line 
```php
# Just empty the string
# $config['auth_source'] = 'ldap';
$config['auth_source'] = '';
```
* Step 4. On `application/config/rest.php` line `113`,  
From empty string, put to `basic`
```php
$config['rest_auth'] = 'basic';
```

* Step 5. On `application/config/rest.php` line `213`,  
Configure available credentials for API Access
```php
$config['rest_valid_logins'] = ['admin' => '1234'];
```


* Step 6. On `application/libraries/REST_Controller.php` line `764`,  
Make custom response for forbidden and unauthorized access
```php
public function response($data = NULL, $http_code = NULL)
   {
ob_start();
       // If the HTTP status is not NULL, then cast as an integer
       if ($http_code !== NULL)
       {
           // So as to be safe later on in the process
           $http_code = (int) $http_code;

           # Forbidden / Unauthorized message
	   if($http_code == 401 || $http_code == 403){
               header("Content-type:application/json");
               http_response_code($http_code);
               $msg = array('message' => ($http_code == 401) ? "Unauthorized" : "Forbidden");
               $this->output->_display(json_encode($msg));
               exit;
	   }
           # / Forbidden / Unauthorized message
       }
       ...
```

* Step 7. (Optional)   
Create `logs` Table for recording every access of the API
```sql
CREATE TABLE `logs` (
       `id` INT(11) NOT NULL AUTO_INCREMENT,
       `uri` VARCHAR(255) NOT NULL,
       `method` VARCHAR(6) NOT NULL,
       `params` TEXT DEFAULT NULL,
       `api_key` VARCHAR(40) NOT NULL,
       `ip_address` VARCHAR(45) NOT NULL,
       `time` INT(11) NOT NULL,
       `rtime` FLOAT DEFAULT NULL,
       `authorized` VARCHAR(1) NOT NULL,
       `response_code` smallint(3) DEFAULT '0',
       PRIMARY KEY (`id`)
   ) ENGINE=InnoDB DEFAULT CHARSET=utf8;
```

* Step 7.1 (Optional) table On `application/config/rest.php` line `406`  
Make logging available
```php
# Make true if you want to use logging
# $config['rest_enable_logging'] = FALSE;
$config['rest_enable_logging'] = TRUE;
```

`Credits to JC sin(π)`

- - -
 
# Accelerated Mobile Pages (AMP)

## For setting dynamic origin
Put this in your API
```php
# For setting dynamic origin
$http_origin = $_SERVER['HTTP_ORIGIN'];
if ($http_origin == "https://alveoland.com.ph" ||
   $http_origin == "https://www.alveoland.com.ph")
header("AMP-Access-Control-Allow-Source-Origin: $http_origin");
# / For setting dynamic origin
```
- - -

# API
## Twitter API
[⬆ Back to top](#dev-cheat-sheet-)
#### Getting tweets from a certain account
```html
<!-- Twitter block -->
<a class="twitter-timeline" data-width="650"
data-height="270" href="https://twitter.com/jjjjcccjjf">Tweets by @jjjjcccjjf</a>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>
<!-- /Twitter block -->
```

---

# Deployment
[⬆ Back to top](#dev-cheat-sheet-)

## Command-line snippets
To be able to fire up these snippets, you must boot up your terminal first. 
On windows, you need to launch [git bash](https://git-scm.com/downloads). On Mac, click on the `spotlight` then type in `terminal`.
  
### Installing Wordpress
Copy and paste the ff. to your Terminal
```bash
cd /path/to/your/environment/
curl -O https://wordpress.org/latest.zip
unzip latest.zip
rm latest.zip
mv wordpress my-project
cd my-project
cp -i wp-config-sample.php wp-config.php
```       

### Setup your Version Control
[⬆ Back to top](#dev-cheat-sheet-)

Assuming you're inside your project directory
```bash
git init
git add .
git commit -m "initial commit"
git remote add origin https://github.com/your-username/my-project.git
git push -u origin master
```

## .htaccess
[⬆ Back to top](#dev-cheat-sheet-)  

#### Regular wordpress htaccess
(Optional) For fixing forbidden in wp-admin
```htaccess
# BEGIN WordPress
# Uncomment this block if you cannot access wp-admin
# <Files wp-login.php>
# Order Deny,Allow
# Deny from all
# Allow from all
# </Files>
# / Uncomment this block if you cannot access wp-admin

# Uncomment this block for blocking wp-admin access except on some IP addresses
# RewriteCond %{REQUEST_URI} ^(.*)?wp-login\.php(.*)$ [OR]
# RewriteCond %{REQUEST_URI} ^(.*)?wp-admin$
# RewriteCond %{REMOTE_ADDR} !^124.106.142.167$
# RewriteRule ^(.*)$ - [R=403,L]

<IfModule mod_rewrite.c>
RewriteEngine On
RewriteBase /
RewriteRule ^index\.php$ - [L]
RewriteCond %{REQUEST_FILENAME} !-f
RewriteCond %{REQUEST_FILENAME} !-d
RewriteRule . /index.php [L]
</IfModule>
# END WordPress
```

### Leverage browser caching
Paste this in your .htaccess anywhere I guess? 😅
The purpose of this block of code is  to set expiration to caching. (maybe) You can read more of the topic [here.](https://developers.google.com/speed/docs/insights/LeverageBrowserCaching)

```htaccess
# Begin CACHE CONTROL
<IfModule mod_expires.c>
    ExpiresActive On
    ExpiresByType text/css A31536000
    ExpiresByType text/x-component A31536000
    ExpiresByType application/x-javascript A31536000
    ExpiresByType application/javascript A31536000
    ExpiresByType text/javascript A31536000
    ExpiresByType text/x-js A31536000
    ExpiresByType text/html A3600
    ExpiresByType text/richtext A3600
    ExpiresByType image/svg+xml A3600
    ExpiresByType text/plain A3600
    ExpiresByType text/xsd A3600
    ExpiresByType text/xsl A3600
    ExpiresByType text/xml A3600
    ExpiresByType video/asf A31536000
    ExpiresByType video/avi A31536000
    ExpiresByType image/bmp A31536000
    ExpiresByType application/java A31536000
    ExpiresByType video/divx A31536000
    ExpiresByType application/msword A31536000
    ExpiresByType application/vnd.ms-fontobject A31536000
    ExpiresByType application/x-msdownload A31536000
    ExpiresByType image/gif A31536000
    ExpiresByType application/x-gzip A31536000
    ExpiresByType image/x-icon A31536000
    ExpiresByType image/jpeg A31536000
    ExpiresByType image/webp A31536000
    ExpiresByType application/json A31536000
    ExpiresByType application/vnd.ms-access A31536000
    ExpiresByType audio/midi A31536000
    ExpiresByType video/quicktime A31536000
    ExpiresByType audio/mpeg A31536000
    ExpiresByType video/mp4 A31536000
    ExpiresByType video/mpeg A31536000
    ExpiresByType application/vnd.ms-project A31536000
    ExpiresByType application/x-font-otf A31536000
    ExpiresByType application/vnd.ms-opentype A31536000
    ExpiresByType application/vnd.oasis.opendocument.database A31536000
    ExpiresByType application/vnd.oasis.opendocument.chart A31536000
    ExpiresByType application/vnd.oasis.opendocument.formula A31536000
    ExpiresByType application/vnd.oasis.opendocument.graphics A31536000
    ExpiresByType application/vnd.oasis.opendocument.presentation A31536000
    ExpiresByType application/vnd.oasis.opendocument.spreadsheet A31536000
    ExpiresByType application/vnd.oasis.opendocument.text A31536000
    ExpiresByType audio/ogg A31536000
    ExpiresByType application/pdf A31536000
    ExpiresByType image/png A31536000
    ExpiresByType application/vnd.ms-powerpoint A31536000
    ExpiresByType audio/x-realaudio A31536000
    ExpiresByType image/svg+xml A31536000
    ExpiresByType application/x-shockwave-flash A31536000
    ExpiresByType application/x-tar A31536000
    ExpiresByType image/tiff A31536000
    ExpiresByType application/x-font-ttf A31536000
    ExpiresByType application/vnd.ms-opentype A31536000
    ExpiresByType audio/wav A31536000
    ExpiresByType audio/wma A31536000
    ExpiresByType application/vnd.ms-write A31536000
    ExpiresByType application/font-woff A31536000
    ExpiresByType application/font-woff2 A31536000
    ExpiresByType application/vnd.ms-excel A31536000
    ExpiresByType application/zip A31536000
</IfModule>
# End CACHE CONTROL
```
