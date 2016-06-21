# WordPress-Migration-Database-Replacement


##Getting Started  
Go to your mysqladmin page. Find the desire database and run these query to replace old domain link.   

- `UPDATE wp_posts SET guid = replace(guid, 'http://olddomain.com','http://newdomain.com');`  
- `UPDATE wp_postmeta SET meta_value = replace(meta_value,'http://olddomain.com','http://newdomain.com');`  
- `UPDATE wp_posts SET post_content = REPLACE(post_content, 'http://olddomain.com', 'http://newdomain.com');`  

Change table prefix `wp_` if you have another table prefix . 

Credit: [https://www.smashingmagazine.com/2016/06/free-ssl-for-any-wordpress-website/](https://www.smashingmagazine.com/2016/06/free-ssl-for-any-wordpress-website/)


