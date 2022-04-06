# All-About-Wordpress
![download](https://user-images.githubusercontent.com/52255671/111907277-c923a180-8a7e-11eb-92b7-31e838009fd6.png)

**1. Wordpress Resources**

      1.  Wp Best Plugin , Themes and etc : https://www.wpsuperstars.net/
      2.  Expert the wordpress following the steps : https://wpnewsify.com/blog/steps-become-wordpress-professional/
      3.  Pro Plugin : https://developerszone.net/
     


**2. Wordpress Installing Problem**
   
    1.  Problem : could not create a directory for plugin
        Command : sudo chmod 777 -R /opt/lampp/htdocs/nayem_tech
        
    2. FTP out : wp-config -> define('FS_METHOD', 'direct');


**3. Elementor Icon Box Mobile Align Css:
@media (max-width: 600px) {
.elementor-icon-box-icon {
float: left;
}

.elementor-icon-box-content {
text-align: left;
margin-left: 50px;
}
}
**4. Elementor Loading Problem: 
First of all have to active and deactive all plugins if it is not work this code will place on the cpanel:

File Max Upload Size:
1. php.ini codes
===============
upload_max_filesize = 256M
post_max_size = 256M
memory_limit = 256M
file_uploads = On
upload_max_filesize = 128M
max_execution_time = 300
max_allowed_packet_size = 524288000

2. .htaccess codes
===================
php_value max_input_vars 5000
php_value max_execution_time 300
php_value post_max_size 128M
php_value upload_max_filesize 128M
php_value memory_limit 256M

3. wp-config.php code
=====================
define( 'WP_MEMORY_LIMIT', '128M' );

