# MyTheme

**MyTheme** is an *easy-to-use*, *customizable* and *responsive* **Ghost**<sup id="t1">[1](#f1)</sup> theme. 
See it in action on www.blog.oliastic.com!

![MyTheme](http://www.blog.oliastic.com:8080/content/images/2015/09/MyTheme_NormalScreen_h380.png)




## Features

* Customizable via single config file
* Responsive design for different screen sizes
* Optional search function
* Additional menu items 
* Configurable comment threads
* Layout options for static pages



## Installation

1. Download the [MyTheme GitHub ZIP](https://github.com/oliastic/MyTheme/archive/master.zip) 
2. Unzip the main folder from the archive to the themes folder of your Ghost installation: `[GHOST-INSTALLATION]/content/themes/MyTheme-master`
3. Rename the folder from `MyTheme-master` to `MyTheme`
4. Restart your Ghost blog
5. Go to the **Ghost Config Environment**: `http://[YOUR-BLOG-URL]/ghost`
6. On the settings page select **MyTheme** under *Themes*
7. Save the settings
8. Follow the instructions below for [configuring](#Configuration) **MyTheme** according to your wishes



## Configuration

### Ghost Config Environment

The following elements configured in the **Ghost Config Environment** (`http://[YOUR-BLOG-URL]/ghost`) are used by **MyTheme**:

* Blog Title
* Blog Description
* Blog Cover
* Posts Per Page
* User Name, Slug, E-Mail, Location, Website, Bio 
* Tag Name, URL, Description, Image
* Navigation Entries

Of course you do not have to define every single one of them, if you do not like some information to show up!






### Basic configuration via config file

**MyTheme** uses a single file file for the basic configuration! 

Open the `config.js` located under

`[GHOST-INSTALLATION]/content/themes/MyTheme/assets/js/`

in a text editor and adapt the settings described below according to your wishes!

---

#### Blog Header

##### `my_theme_do_hide_blogtitle`

Value: ***true*** or ***false*** (default)

Set to ***true*** if no **Blog Title**e should appear in the **Blog Header**. This is useful when using a **Blog Logo** that contains the title of the blog itself.



##### `my_theme_do_hide_blogdescription`

Value: ***true*** or ***false*** (default)

Set to ***true*** if no **Blog Description** should appear in the **Blog Header**. This is useful when using a **Blog Logo** that contains the description of the blog itself.



##### `my_theme_do_align_bloglogo_vertically`

Value: ***true*** or ***false*** (default)

Set to ***true*** if the **Blog Logo** should be aligned vertically in front of the **Blog Title**, set to ***false*** to align the **Blog Logo** horizontally before the **Blog Title**.



#### Search Field

##### `my_theme_do_display_search_field`

Value: ***true*** (default) or ***false***

Set to ***true*** if a search field based on **GhostHunter**<sup id="t2">[2](#f2)</sup> should be displayed to the navigation menu.


##### `my_theme_do_display_search_field_in_separate_row`

Value: ***true*** (default) or ***false***

Set to ***true*** if a search field should be displayed in a separate row within the navigation. 



#### Bonus Pages

**MyTheme** allows you to define up to 3 additional bonus pages. 
All regular menu items (defined in the **Ghost Config Environment**)  will appear on the left side (or on the top for small screens) of the navigation menu.
All bonus pages will appear on the right side (or on the bottom for small screens) of the navigation menu. 

##### `my_theme_bonus_page_name_1`, `my_theme_bonus_page_name_2`, `my_theme_bonus_page_name_3`

Value: **[STRING]** (default: "")

Short name of the page that appears in the navigation menu (e.g. `About`).

##### `my_theme_bonus_page_link_1`, `my_theme_bonus_page_link_2`, `my_theme_bonus_page_link_3`

Value: **[STRING]** (default: "")

Relative or absolute link to the page (e.g. `/about` or `http://[SOME-URL]`). 




#### Static Pages

##### `my_theme_static_page_do_show_time_stamp`

Value: ***true*** or ***false*** (default)

Set to ***true*** if time stamp should be displayed at the top of static pages.


##### `my_theme_static_page_do_show_share_links`

Value: ***true*** or ***false*** (default)

Set to ***true*** if share links should be displayed at the bottom of static pages.


##### `my_theme_static_page_do_show_author_info`

Value: ***true*** or ***false*** (default)

Set to ***true*** if author information should be displayed at the bottom of static pages.


##### `my_theme_static_page_do_show_comments`

Value: ***true*** or ***false*** (default)

Set to ***true*** if comments should be displayed at the bottom of a static pages. 
(Comments in general must be activated too! See below!) 



#### Comments

##### `my_theme_disqus_do_activate_comments`

Value: ***true*** or ***false*** (default)

Set to ***true*** if **Disqus**<sup id="t3">[3](#f3)</sup> comments should be displayed at the bottom of posts.



##### `my_theme_disqus_do_create_thread_per_post`

Value: ***true*** or ***false*** (default)

Set to ***true*** if a separate comment thread should be created for each page. 
Set to ***false*** to use one global comment thread shared by all posts of your blog.


##### `my_theme_disqus_shortname`

Value: **[STRING]** (default: "")

Set to your registered **Disqus Shortname**!


##### `my_theme_disqus_identifier`

Value: **[STRING]** (default: "")

Set to a unique word associated with your blog (e.g. your blog title). That way, a change of the blog url will not lead to new comment thread created by **Disqus**.
If separate threads for each post are activated (see above), **MyTheme** will automatically extend the **Disqus Identifier** by the *ID* of the current post. 



### Additional configuration


#### Favicon

Just replace the `favicon.ico' located under

`[GHOST-INSTALLATION]/content/themes/MyTheme/assets/`

with your own **Favicon Icon**!




#### Style Sheet

To further adapt the design and layout of **MyTheme** according to your wishes edit the `style_default.css` located under  

`[GHOST-INSTALLATION]/content/themes/MyTheme/assets/css/`

**Hint:** Right at the top of the style sheet you will find a section called `DESIGN COLORS AND FONTS`! 



## Further Remarks

* **MyTheme** is published under **The MIT License (MIT)**<sup id="t4">[4](#f4)</sup>
* Of course you can use and change **MyTheme** as you like 
* It would be nice, if you leave the short **reference to my website** in the footer (or instead add a reference to my website somewhere else). Thanks!

But now, have fun blogging, coding or whatever!

---

<a id="f1">1.</a> Visit https://ghost.org [↩](#t1)

<a id="f2">2.</a> Visit https://github.com/jamalneufeld/ghostHunter [↩](#t2)

<a id="f3">3.</a> Visit https://disqus.com [↩](#t3)

<a id="f4">4.</a> Visit https://opensource.org/licenses/MIT [↩](#t4)


