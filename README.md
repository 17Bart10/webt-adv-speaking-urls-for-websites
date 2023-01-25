# WEBT | ADV | Speaking URLs for websites

## Overview
Apply this advanced user stories to a fitting CORE scenario of your choice.

## User Story 1
*As a Developer I want to setup a rewriting module on my webserver, so that I can rewrite urls.*

### Acceptance Criteria
- A rewrite module is installed and ready for use on the webserver

## User Story 2
*As a Developer I want to offer speaking URLs for all pages of my website, so that search engines rank the page higher.*

### Acceptance Criteria
- All pages of the website are reachable via speaking url, including parameters

## How to enable mod_rewrite
- Open the XAMPP/MAMP Apache config File -> "MAMP/conf/apache/httpd.conf"
- Find **`#LoadModule rewrite_module modules/mod_rewrite.so`**
- Delete the "#"
- Find all occourences of **`AllowOverride None`** change it to **`AllowOverride All`**
- Add an `.htaccess` File
- .htacces content  
```
RewriteEngine on
#RewriteRule Pattern Substitution [Optional Flags]
RewriteRule ^my-old-url.html$ /my-new-url.html
```
- Syntax for `.htaccess` `RewriteRule Pattern Substitution [Optional Flags]`
- At last restart the Apache Server (XAMPP/MAMP)  
- Based on the tutorials:
    - https://www.elated.com/mod-rewrite-tutorial-for-absolute-beginners/
    - https://ubiq.co/tech-blog/how-to-enable-mod_rewrite-in-xampp-wamp/

## Updated URLs
- http://dev.webt.local:8888/webt-core-working-with-json-server-responses-in-javascript/UserStoryOne
- http://dev.webt.local:8888/webt-core-working-with-json-server-responses-in-javascript/UserStoryTwo
- http://dev.webt.local:8888/webt-core-working-with-json-server-responses-in-javascript/UserStoryThree
- http://dev.webt.local:8888/webt-core-working-with-json-server-responses-in-javascript/UserStoryFour


#### Links
https://my.skilldisplay.eu/en/skillset/96

---

# WEBT | CORE | Working with JSON Server Responses in JavaScript -> Base for Advanced

## How to build and run TailwindCSS
`npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch`

## Overview
The WIFI Vienna wants to help people who are unsatisfied with their job to choose a random new career path. They require an application which lets you define certain parameters and then presents users of the WebApp with a random job and details on training for it.

## User Story 1
*As a Developer I want to create a proof of concept for an Asynchronous JavaScript (AJAX) request, so that I can continue development based on the prototype.*

### Acceptance Criteria
- An index.html file exists
- The JavaScript “fetch” function is used to fetch dummy data from https://jsonplaceholder.typicode.com/todos/1
- The dummy data fetched is displayed on the page!

## User Story 2
*As a Developer I want to fetch all data from the client's service and display it on the page or console, so that I can later choose random data from the available information.*

### Acceptance Criteria
- The JavaScript “fetch” function is used to fetch the client's data from http://opendata.wifi.at/OpenJsonData.json
- The full dataset is displayed on the page or console to ensure integrity

## User Story 3
*As a Customer I want to push a “Get random Career” button and receive a suggestion for my next job, so that I can restructure my life based on the luck of the draw.*

### Acceptance Criteria
- A random entry is picked from an existing array/list of jobs
- The job is displayed on the page
- The page uses a responsive framework

## User Story 4
*As a Customer I want to have a single job displayed on the screen prominently, featuring title, place of work and description, so that I can identify the relevant information quickly.*

### Acceptance Criteria
- A single job entry is displayed on the page
- The page is responsive
- The page follows the heuristics for user interface design of Jakob Nielsen

#### Links
https://my.skilldisplay.eu/en/skillset/83




