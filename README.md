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
8. multimedia like image, audio, gallery are first class citizens like article
9. serialization to other formats - HTML with embedded images, ePub (native, not convert which is hard to handle)
10. passive social functions - can see referrers, search engines, sends and receives pingbacks and webmentions
11. active social functions - RSS exports, publish to Facebook or YouTube automatically via API, keep videos synchronized with YouTube, comments
12. audit trail - see history of posts, pages, articles
13. antispam - bot called "assuming control" which handles junk and rate limiters everywhere
14. embedded analytics, is aware of article or image
15. multilanguage support
16. heavy inclusion of metadata - OpenGraph, Twitter cards, Pinterest things, microformats, microdata
    into pages, because SEO and we also want to be visible to the world
17. private sections of the site (password protected)
18. caching for pages and images
19. language analysis - detect the language of article, highlight unknown/unusual words as italic (e.g. LibreOffice), do spelling
22. typography - detect double spaces and similar wrongs, replace quotes with language specific ones, but not in source code

## More Details

### 0. be the best web content management system

i have a *not invented here* syndrome in regards of CMSes. Creating and tracking the content must be easy and I must feel happy and without rage and doubts. And my content must be MINE and wasy to work with. It must have a zen feeling

Anyways, I'm sure that I'm not the only one person on this planet not satisfied with the current state of web CMSes or SaaS like Wordpress, Medium, Tumblr

### 1. keep it simple

the system has defined flows, use cases and a clear vision. Refactor regularly and delete and polish the code. Keep it simple, but functional like katana

i've seen enough bloated software in my short life. Websites frozen in time, because the code and technology reached that critial point when adding or changing stuff gets very expensive (days or weeks of work at least)

i'm lazy. You're lazy. I don't have time and mood to maintain dead weight if I know how to simplify it. Simpler code = less code = more fun and more agility. Also it's easier to keep the big picture in head

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

### 6. content can be backed up to local computer easily, including multimedia

the content is the most important thing. It cannot get lost or get corrupted. It is fast to copy it to another machine or local computer

i don't care if something is hard to extract, because it's stored in MySQL database. Fuck, just write the tools to make the problem trivial and easy

### 7. the support for Markdown, Textile, HTML, plaintext and LaTeX formulas out of the box (both source and WYSIWYG)

i like the choice. Markdown is great for technical texts and texts with a simpler formatting, but there's more. Also I'd like to write LaTeX formulas...The system renders the text in realtime. Writing in source code is a preffered way to write texts, but there must be also a WYSIWYG option

HTML editors are horrible. Markdown is usually great, but boring and limiting after some time. Mixing it with HTML is...scary. Bbcode is dead

### 8. multimedia like image, audio, gallery are first class citizens like article

you can add images, audio, galleries like articles along with metadata and all that stuff. Tools are perfect, cropping image, thumbnails

i'd like to add an image and not a empty article with attached image. That's weird, but quite common way to do these things. Do I really need to use Soundcloud to share my audio, because their interface is the best (and the only sane). Do I really need to upload video to YouTube, because custom video players are weird looking and don't work properly half of time? Not really anymore

### 9. serialization to other formats - HTML with embedded images, ePub (native, not convert which is hard to handle), escaped shell sequence, JSON, XML, ...

it's nice and essential to offer to serialize the content to formats which are easy to take offline and copy, HTML with embedded images and CSS, ePub. Also this is mostly a web CMS, but other portals are possible like shell (terminal) access, email access, irc access...

i cannot write my frustrations to this point, because I've never seen it somewhere

### 10. passive social functions - can see referrers, search engines, sends and receives pingbacks and webmentions

the system tracks passive social opportunities from http headers and supports pingbacks, webmentions and similar system-to-system technologies

yaaay! why bother to write stuff, when I cannot see the reach? Actually I'd write even without it, but feedback is nice
5
### 11. active social functions - RSS exports, publish to Facebook or YouTube automatically via API, keep videos synchronized with YouTube, comments

in the end the system is independent of third parties, but can share the content on multiple sites like YouTube and Vimeo for video, soundcloud for audio, images on Deviantart, provide news on Facebook page and so on. Be like a big octopus with one head and lots of tentacles!

because why not? at least for most of the stuff

also comments, there are comments and comments are aggregated also from 3rd party sites, because I'm lazy to browse 10 different sites

### 12. audit trail - see history of posts, pages, articles

the system has an audit trail. Good and usable. When things go wrong, audit trail is a must. Or just to watch the changes

I've never seen a good audit trail. Only like mediocre ones. I'm not surprised, because implementation is hard. Event bus? Proper granularity of classes? Classes cannot do too much (which is fine!)

### 13. antispam - bot called "assuming control" which handles junk and rate limiters everywhere

antispam is a must. Now in 2016 AI is so hyped along with chatbots - consider to surf the wave. Also a security and protection is inherited in the system. Use rate limiters

there's no funnier thing than to see helpless wordpress blog to be spammed with links and fake comments. Or phpBB forums. Very "funny"

### 14. embedded analytics, is aware of article or image

belongs under 5., but is important enough to have own declaration. Analytics interface is essential to track the life of the web site and of the content. It serves also for our narcisstic side to show us how glorious we are. Also for seeing the impact of our troll article or our marketing campaign.

Google analyics is fine I guess. While I never used it much, I always imagined much simpler interface and I couldn't work with that shit every day. Piwik is also fine, but the interface is too big, complex and wasting space. I imagine something more simpler, less "dashboardy".

### 15. multilanguage support

internatiolization and localization are fun. Hard to do right - I like the approach of a full locale - language-country. User interface usually needs only a language except for situations like brazilian portugese language. Anyways UI shoould be in multiple languages, but also system can filter articles by language. There's another thing - Slovak and Czech languages are so close that is makes sense to show content in both languages for either locale. Small details, but important

### 16. heavy inclusion of metadata - OpenGraph, Twitter cards, Pinterest things, microformats, microdata into pages, because SEO and we also want to be visible to the world

findability is like the most important thing right now. Why to hide our awesome content? Also the system shows a preview of twitter cards or facebook so I can see that the cover image is ok.

i'm frustrated only about microdata, because that spec is fucking long and complex and I don't know where it shows results. Like somewhere at Google search, maybe other services. We'll see

### 17. private sections of the site (hidden from navigation or password protected)

i like to write stuff that is made for certain person or small group of people. Like look what a bug. Or some really personal feelings. The system is for sharing, right?

### 18. caching for pages and images

ultimately the system is as fast as possible. Use caching, but use some easy and manageable way to do it

### 19. language analysis - detect the language of article, highlight unknown/unusual words as italic (e.g. LibreOffice), do spelling

provide luxury and automate everything until it pains and then a little more

nobody wants to work with a shitty system and do the same things for more than year or two. Zen, remember, zen experience

### 22. typography - detect double spaces and similar wrongs, replace quotes with language specific ones, but not in source code

there are options to provide *automatic* luxury of typography as seen in books. Why automatic? UTF-8 table has like 20 different "-" and like a milion different quotes and apostrophes. The consistency is better looking than fancy quote here and there


