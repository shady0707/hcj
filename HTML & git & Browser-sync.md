# HTML & git & Browser-sync

1. commit local files to remote git:

   $ git add .     *. means everything, or substitute it with file name, this mark the files need to be committed later*

   $ git commit -m "*some notes*".     *commit files to github (remote site)*

   $ git push     *update the remote site with local site files*

   $ git status    *check the status to see if everything committed*

   $ git config --get remote.origin.url *look for the original url of this repo*
2. browser-sync 

   $browser-sync start --server --files "*"    *"\*"is the file you wanna keep updated*

   then go to localhost:3000/* ,it will keep updated while you edit.

3. pseudo-class selector:

   selector : pseudo-class {}

4. alwasy escape: <, >, &, 
   use **&lt;**, **&gt;**, **&amp;** instead

5. \<section>: a generic secion of a document, typically with a heading. An introduction, content, or contact information can be a section.  
    \<div>: no special meaning. When no other element is suitable, choose this one (poor accessibility). **block element** .  
    \<span>:  in-line element.   
    \<article>: indipendent item section of content, **must have \<h1> tag as title**. Such as a blog post, newspaper article, etc. It's an independent content.  
    \<nav>: navigation links.  
    \<p>: a paragraph, automatically add a single blank line before and after each \<p> element.
    >

# Useful prototype codes of css
1. In line style  
   ```html
   <p style='color: green; font-size: 20px;'></p>
   <p class='mainpoint highlight class_name'></p>
   ```

2. list  
   ```html
   <ol>  
      <li>  
      <li>
   </ol>

   <ul>
      <li>
      <li>
   </ul>
   ```

3. Links  
   ```html
   <a href='http://aaa.com'>aaa</a>
   <a herf='http://bbb.com' target='_blank' title='xxxx'>bbb</a>

4. img 
   ```html
   <img src='xxx.jpg' width='111' height='222' alt='some words'>

5. selectors  
   ```css
   /*all h1 and p elements*/
   h1, p {

   } 

   /*all with class='class_name'*/
   .class_name {

   } 

   /*all with id='id_name'*/
   #id_name {

   } 

   /*all h2 element directly under section*/
   section > h2 {

   } 

   /*all li under section*/
   section li{

   } 

   /*all p with class='class_name'*/
   p.class_name {

   } 

   /*all elements with class='mainpoint' and class='highlight'*/
   .mainpoint.highlight {

   } 

   /*The odd th child of div under section
   section div:nth-child(odd) {

   }

   /*higher priority feature*/
   p {
      color: green; !important;
   }

   /*The most important*/
   * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
   }

   /*background with image*/
   #bg {
      width: 100px;
      height: 100px;
      background: url('xxx.png') no-repeat center top;
      background-color: blue;
   }

6. Float
   ```css
   #p1 {
      width: 50%; 
      float: right;
      clear: both;
   }

7. Positioning
   ```css
   #p1 {
      position: relative;
      top: 65px;
      left: 65px;
   }

   #p3 {
      position: absolute;
      top: 0;
      left: 0;
   }

8. Media query
   ```css
   @media (min-width: 992px) and (max-width: 1199px) {
      #p1 {
         width: 100%;
      }

      #p2 {

      }
   }

9. Responsive
   ```css
   @media (min-width: 1200px) {
      .col-lg-1, .col-lg-2, .col-lg-3, .col-lg-4, .col-lg-5, .col-lg-6, .col-lg-7, .col-lg-8, .col-lg-9, .col-lg-10, .col-lg-11, .col-lg-12 {
         float: left;
      }
      .col-lg-1 {
         width: 8.33%;
        }
        .col-lg-2 {
            width: 16.66%;
        }
        .col-lg-3 {
            width: 25%;
        }
        .col-lg-4 {
            width: 33.33%;
        }
        .col-lg-5 {
            width: 41.66%;
        }
        .col-lg-6 {
            width: 50%;
        }
        .col-lg-7 {
            width: 58.33%;
        }
        .col-lg-8 {
            width: 66.66%;
        }
        .col-lg-9 {
            width: 74.99%;
        }
        .col-lg-10 {
            width: 83.33%;
        }
        .col-lg-11 {
            width: 91.66%;
        }
        .col-lg-12 {
            width: 100%;
        }
      @media (min-width: 992px) and (max-width: 1199px) {
     .col-md-1, .col-md-2, .col-md-3, .col-md-4, .col-md-5, .col-md-6, .col-md-7, .col-md-8, .col-md-9, .col-md-10, .col-md-11, .col-md-12 {
      float: left;
      border: 1px solid green;
      }
      .col-md-1 {
         width: 8.33%;
      }
      .col-md-2 {
         width: 16.66%;
      }
      .col-md-3 {
         width: 25%;
      }
      .col-md-4 {
         width: 33.33%;
      }
      .col-md-5 {
         width: 41.66%;
      }
      .col-md-6 {
         width: 50%;
      }
      .col-md-7 {
         width: 58.33%;
      }
      .col-md-8 {
         width: 66.66%;
      }
      .col-md-9 {
         width: 74.99%;
      }
      .col-md-10 {
         width: 83.33%;
      }
      .col-md-11 {
         width: 91.66%;
      }
      .col-md-12 {
         width: 100%;
      }
   }
 