# Enzo's Dev Cheetsheet

---

# Table of Contents 
## Development Tools
1. Text Editors / Integrated Development Environment (IDE)
    1. Atom
    1. Sublime
    1. Visual Studio Code
1. Chrome Extensions
    1. [var_masterpiece](https://chrome.google.com/webstore/detail/varmasterpiece/chfhddogiigmfpkcmgfpolalagdcamkl?utm_source=chrome-app-launcher-info-dialog)
    1. [JSON Formatter](https://chrome.google.com/webstore/detail/bcjindcccaagfpapjjmafapmmgkkhgoa?utm_source=chrome-app-launcher-info-dialog)
1. File Transfer Clients
   1. FIlezilla
1. Version Control Clients
   1. SourceTree
   1. Git Kraken
   1. Git Bash (Terminal Interface)

## Front-end
1. [CSS Snippets](#css-snippets)
1. [Animation Snippets](#animation-snippets)

## Back-end
1. [PHP Snippets](#php-snippets)
    1. [Wordpress](#snippets)
        * [Installing Wordpress](#installing-wordpress)
        * [Branding your theme](#branding-your-theme)
        * [Common wordpress plugins](#common-wordpress-plugins)
        * [Wordpress Snippets](#wordpress-snippets)
    1. Generic PHP Snippets
1. JavaScript Snippets

## Cheatsheets
1. Git Cheatsheet
1. Markdown Cheatsheet

## Deployment
1. Command-line snippets
    * [Installing Wordpress](#installing-wordpress)
    * [Setup your version control](#setup-your-version-control)
1. .htaccess
* * *

# CSS Snippets

For controlling re-captcha css
```css
#rc-imageselect, .g-recaptcha {transform:scale(0.8);-webkit-transform:scale(0.8);transform-origin:0 0;-webkit-transform-origin:0 0;}
```

---

# Development Tools

## Text Editors / Integrated Development Environment (IDE)
## Atom
##### About
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

## Sublime
#### About
I don't use sublime that much. But it's blazingly faster compared to other text editors.
#### Pros:
* Super fast
#### Cons: 
* Installing packages is such a hassle
#### Recommended Packages:
* TODO:

[View Website](https://www.sublimetext.com/)
## Visual Studio Code
#### About
Haven't used this much yet. So I don't have much opinion about it.

[View Website](https://code.visualstudio.com/)
* * * 

# PHP Snippets
## Number formatting

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


* * * 

## Animation Snippets
### Smooth scrolling on anchors on the same page
Just paste this on your footer and it will work

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

* * * 

# Command-line snippets
Open Terminal  / TODO Windows + R or Command + R
  
## Installing Wordpress

Copy and paste the ff. to your Terminal

       cd /path/to/your/environment/
       curl -O https://wordpress.org/latest.zip
       unzip latest.zip
       rm latest.zip
       mv wordpress my-project
       cd my-project
       cp -i wp-config-sample.php wp-config.php

## Setup your Version Control
Assuming you're inside your project directory
       
       git init
       git add .
       git commit -m "initial commit"
       git remote add origin https://github.com/your-username/my-project.git
       git push -u origin master

* * *

# .htaccess
Regular Wordpress .htaccess. 
(Optional) For fixing forbidden in wp-admin

       # BEGIN WordPress
       # Uncomment this block if you cannot access wp-admin
       # <Files wp-login.php>
       # Order Deny,Allow
       # Deny from all
       # Allow from all
       # </Files>
       # / Uncomment this block if you cannot access wp-admin
       <IfModule mod_rewrite.c>
       RewriteEngine On
       RewriteBase /
       RewriteRule ^index\.php$ - [L]
       RewriteCond %{REQUEST_FILENAME} !-f
       RewriteCond %{REQUEST_FILENAME} !-d
       RewriteRule . /index.php [L]
       </IfModule>
       # END WordPress

* * * 

# Wordpress Snippets

After [installing wordpress](#installing-wordpress), edit your `wp-config.php` and fill-out appropriate credentials
       
## Branding your theme
 
1. Delete all themes except the latest one
1. Rename the theme to your desired theme name
1. In your theme directory, open `style.css`
1. On `line 2`, replace `Theme Name: Twentyseventeen` to `Theme Name: Your Theme Name`
1. Delete all styles (Because this will override your custom theme style)

or you can just run this script...

       cd wp-content
       cd themes
       rm twentyfifteen -r
       rm twentysixteen -r
       mv twentyseventeen my-project 
       sed -i -e 's/Twenty Seventeen/my-project/g' my-project/style.css
       sed -i '16,$d' my-project/style.css
       rm my-project/style.css.bak

### Setup a Front Page
1. Copy and replace the contents of `front-page.php` with this.
       
       <?php
       /* Template Name: Home */
       get_header();
       while(have_posts()): the_post();
       ?>
       
       <!-- your content here ->
       
       <?php 
       endwhile;
       get_footer();
       
1. Create a page and let it have a `Home` template    
1. Go to Settings > Reading
1. On the `Front page displays` section, tick `A static page` radio
1. On the drop down, select `Home` template as Front page
1. Save changes

### Header and Footer
1. Personalize your `header.php` and `footer.php`
1. Don't forget to put `<?php wp_head(); ?>` before the closing `</head>` of your header tag
1. Don't forget to put `<?php wp_footer(); ?>` before the closing `</body>` of your body tag
1. Replace/Import your assets (css, js, images) inside `/your-theme-name/assets/` folder
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
       
 1. Use this script for dynamic url in our includes
       
        <link rel="stylesheet" href="<?php echo get_template_directory_uri(); ?>/assets/css/styles.css">
	
## Wordpress Plugins

### Common wordpress plugins.
Common WP plugins for a generic website

| Plugin name                           | Description                                  |
| ------------------------------------- | -------------------------------------------- |
| Contact Form 7                        | Most common plugin for contact forms         |
| Contact Form 7 Database Addon – CFDB7 | Save contact form submissions to wp-admin    |
| Custom Post Type UI                   | For custom post types                        |
| [Advanced Custom Fields PRO](https://drive.google.com/file/d/0B_bwOHDZvZw-UkJZYUxRRWFHUUE/view?usp=sharing) | For additional custom fields                 |  
| Enable Media Replace | For replacing images in Media Library |

### Advanced wordpress plugins
TODO

## Wordpress Snippets

### 「ＴＨＥ ＬＯＯＰ」

       <?php
       /* Template Name: My Template */
       get_header();
       while(have_posts()): the_post();
       ?>

       <!-- your content here -->

       <?php 
       endwhile;
       get_footer();

### Linking to assets

       <link rel="stylesheet" href="<?php echo get_template_directory_uri(); ?>/assets/css/styles.css">

### Basic loop for iterating posts

       <?php
       $args = array('post_type' => 'service', 'posts_per_page' => -1);
       $the_query = new WP_Query($args);
       if ( $the_query->have_posts() ) {  while ( $the_query->have_posts() ): $the_query->the_post(); ?>
        <!-- your content here -->
       <?php endwhile; wp_reset_postdata(); } else { /** no posts found **/ } ?>
       
### Basic Loop with optional meta query
       
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
       
       
### Get WP nav menu items

       /** variable for our menu object **/
       $menu_obj = wp_get_nav_menu_items('main'); # wp post object for `main` wp menu

       <!-- menu loop -->
       <?php foreach ($menu_obj as $obj): ?>
           <li><a href="<?= $obj->url; ?>"><?= $obj->title; ?></a></li>
       <?php endforeach; ?>
       <!-- /menu loop -->
       
### Add Shortcode in your template

      <?php echo do_shortcode('[contact-form-7 id="89" title="Food Tasting"]'); ?>
 
### Advanced Custom Fields Simple Repeater Loop

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
 
### Advanced Custom Fields Nested Repeater Loop 
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
         <?php $child_repeater_obj = $venue['child_repeater_field_name'];
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

       $path = $_SERVER['DOCUMENT_ROOT'] . '/wealthmart'; #TODO: Change me on live

       include_once $path . '/wp-config.php';
       include_once $path . '/wp-load.php';
       include_once $path . '/wp-includes/wp-db.php';
       include_once $path . '/wp-includes/pluggable.php';


#### Displaying `the_content` with formatting (normally, it doesn't display formatting)
       
       <?php echo apply_filters('the_content', get_post_field('post_content', 92)); ?>
       
#### Detect if page is of custom post type or single

	if(is_singular(array('cpt_name'))){
	}
	
#### Args for searching WP Query

        $args = array('post_type' => array('page', 'project', 'location', 'bank'),
         'posts_per_page' => -1, 's' => @$_GET['q']);

#### Display post count from the WP Query

       $args = array('post_type' => 'service', 'posts_per_page' => -1);
       $the_query = new WP_Query($args);
       echo $the_query->post_count; # The post count
	 
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

## Pagination

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
    'base'            => get_pagenum_link(1) . '%_%',
    'format'          => 'page/%#%',
    'total'           => $numpages,
    'current'         => $paged,
    'show_all'        => False,
    'end_size'        => 1,
    'mid_size'        => $pagerange,
    'prev_next'       => True,
    'prev_text'       => __('&laquo;'),
    'next_text'       => __('&raquo;'),
    'type'            => 'plain',
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
$loop = new WP_Query( $args );
if ($loop->have_posts()) : while ( $loop->have_posts() ) : $loop->the_post();
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
  custom_pagination($loop->max_num_pages,"",$paged);
}
# Make sure to change $loop variable to your actual loop variable!!!!
/* Pagination */
wp_reset_postdata();
?>
``` 
