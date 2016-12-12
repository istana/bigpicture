# bigpicture

## Star Mammoth manifesto

0. be the best content management system in the Internet with regard to the following rules
1. keep it simple
2. all data are serializable to JSON documents
3. themeable, highly customizable
4. intuitive text formatting or multimedia upload
5. comfortable administration, statistics and monitoring interface

6. content can be backed up to local computer easily, including multimedia
7. the support for Markdown, Textile, HTML, plaintext and LaTeX formulas out of the box (both source and WYSIWYG)
8. multimedia like image, audio, gallery are first class citizens like article,
   uploading and processing of multimedia is easy and automatic
9. serialization to other formats - HTML with embedded images, ePub (native, not convert which is hard to handle),
   escaped shell sequence, JSON, XML, ...
10. passive social functions - can see referrers, search engines, sends and receives pingbacks and webmentions
11. active social functions - RSS exports, publish to Facebook or YouTube automatically via API,
   keep videos synchronized with YouTube, comments
12. audit trail - see history of posts, pages, articles, ...
13. antispam - bot called "assuming control" which handles junk and rate limiters everywhere
14. embedded analytics, is aware of article or image
15. multilanguage support
16. heavy inclusion of metadata - OpenGraph, Twitter cards, Pinterest things, microformats, microdata
    into pages, because SEO and we also want to be visible to the world
17. private sections of the site (password protected)
18. caching for pages and images
19. independent of third parties, but possibility to use them. YouTube for videos, gists for source code, deviantart for images... 
20. language analysis - detect the language of article, highlight unknown/unusual words as italic (e.g. LibreOffice), do spelling
21. typography - detect double spaces and similar wrongs, replace quotes with language specific ones, but not in source code

## More Details

### 0. be the best web content management system

i have a *not invented here* syndrome in regards of CMSes. Creating and tracking the content must be easy and I must feel happy and without rage and doubts. And my content must be MINE and wasy to work with. It must have a zen feeling

Anyways, I'm sure that I'm not the only one person on this planet not satisfied with the current state of web CMSes or SaaS like Wordpress, Medium, Tumblr

### 1. keep it simple

the system has defined flows, use cases and a clear vision. Refactor regularly and delete and polish the code. Keep it simple, but functional like katana

i've seen enough bloated software in my short life. Websites frozen in time, because the code and technology reached that critial point when adding or changing stuff gets very expensive (days or weeks of work at least)

### 2. all data are serializable to JSON documents

this makes a migration to a new generation of CMS of another system without diving into insanity. Relations are included in the JSON document - e.g. an article together with embedded images encoded in (base64). Use JSON schema to generate and validate the document. This makes versions of JSON export more manageable

i've experienced endless of pain upgrading Zencart and Prestashop. Generally I wasn't successful. Fuck this shit. You must never be required to scrap all your data and start anew - and spend a month to enter old data via web interface or something, because untangle that database dump is pain in the ass. And CP-1250 as encoding for strings sucks

### 3. themeable, highly customizable

there is a support for themes - the system is multifacial, i.e. different layouts for different sections of the website

we require you to use Material design or bright colors or Human interface...fuck that. I liked Material design, but I've grown weary of it. I like dark backgrounds and evolving designs. And different designs.

### 4. intuitive text formatting or multimedia upload

writing of text and formatting is easy and fast including design of sections, header and styles in general. Upload of images and other multimedia is easy and automatic. Support at least HTML, Markdown and Textile formatting

really, focus on writing stuff and adding metadata. Asking for URL if I want to add an image is insane, unless the system copies it to the database. But usually I want to upload my own stuff

### 5. comfortable administration, statistics and monitoring interface

administration is the part where you as a content creator spend the most of time. It has to be the best and the easiest to use and configure. Statistics are important, because I want to know how many people saw that article, which web browers do they use, which countries are they from. Guestbooks and shoutboxes are dead. 95% visitors are like ghosts, they won't write a message or email, they just fly around and then leave. Monitoring is important to track the content during its life. Dead links, pingbacks, changes

without proper administration the system is useless and fuck that, you will spend hours to do even simple things like formatting an article or deleting spam comments one by one, because there's no antispam and the sytem doesn't allow mass delete




