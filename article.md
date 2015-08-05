# Fedora developer portal

Fedora developer portal has arised as idea from Mr. Josef Stribny and Mr. Petr Hracek. The aim of the portal is to give an overview about important development tools or projects in Fedora. Focus is targeted to beginners, advanced users or developers.   
Can we ask question why to have that portal?  
 Answer is really simple. In order that we make easy developers to develop applications on Fedora either on Fedora Workstation, Server or Cloud.   
Therefore it is needed to show and advise users how to use Fedora for given area. Sort of if we are able to cover a set of areas then Fedora will be pleasanter for users and developers.

## For whom Fedora developer portal should serve for?

Fedora developer portal has the aim to make easy Fedora users as from developer point of view as to introduce new things which are available in Fedora. Fedora user therefore will have the overview:

*   about new technologies,
*   about available developer languages,
*   about projects released in each Fedora release cycle,
*   about important tools in Fedora (like Docker, Vagrant, DevAssistant etc.),
*   about tools which can be used for development.

Portal should be of course used for users which would like to develop applications on Fedora. Each section, for which is user interested on, provides a guide how to setup environment or system for given area.

Nowadays portal looks like in following picture or directly on portal [https://developer-phracek.rhcloud.com/](https://developer-phracek.rhcloud.com/). However portal is still under development, and therefore, design of pages is going to redesign.

![](./Fedora_developer_portal_main.png)

What is contents of Powerful Tools in Fedora can be seen on following picture or here [https://developer-phracek.rhcloud.com/tools.html](https://developer-phracek.rhcloud.com/tools.html).

![](./Fedora_developer_portal_tools.png)

## How to write a content for specific area?

It is needed to cover parts with guides in order to provide condidates enough information about developement in Fedora. How to create a given area is described below.

### How to clone portal

Whole portal content is placed on GitHub repository [https://github.com/developer-portal/content](https://github.com/developer-portal/content). It is prerequisite to _fork_ our GitHub repository and clone the portal to your system.  
 This command can be used for it:

<pre>  git clone git@github.com:{your_github_name}/content.git
  </pre>

### How to cover specific area?

Each section must begin with mark in configuration language YAML, which says where relevant area belongs to. For main page **ruby** it is e.g.:

<pre>  ---
  title: Ruby
  page: ruby
  section: tech-languages
  </pre>

Each page, except main page, should have syntax like:

<pre>  ---
  title: Some another text which belongs to ruby
  page: ruby
  ---
  </pre>

The itself is written in [MarkDown](https://en.wikipedia.org/wiki/Markdown) language.

### How to write a portal directly on GitHub pages

Select a part which you would like to create, e.g. nodejs [https://github.com/developer-portal/content/tree/master/tech/languages/nodejs](https://github.com/developer-portal/content/tree/master/tech/languages/nodejs).

*   Press on **+** (which is mentioned after nodejs) which means create a new file and write down a name of the file
*   Provide a content.
*   When the content is finished then press on button "Propose a new file".
*   It saves the content to GitHub and shows you if you would like to create a Pull Request.
*   Press on "Pull Request" and write a description about it.

Next step is on Fedora Developer Portal team to review it and inform you if something should be changed.

### What is missing nowadays

Fedora Developer portal does not have following parts:

*   Tools - DevAssistant, Docker, Vagrant
*   Programming languages - Python, Php, Perl, Go, C, NodeJS, Java
*   databases - PostgreSQL, MariaDB, SQLite
*   Deployment - Copr, SCL, Nulecule, xdgapp, rolekit, openshift
*   Fedora Next

Parts which doesn't have a contant can be found on GitHub here [https://github.com/developer-portal/content/issues](https://github.com/developer-portal/content/issues).

### How to publish your content?

If user covers the part then it should be send to GitHub via Pull Request and send then to portal developers to review. Developers given part verified and eventually send a feedback what to make it better.

### Ruby example on portal

As a example we can show a ruby part, which is already available on portal [https://github.com/developer-portal/content/tree/master/languages/ruby](https://github.com/developer-portal/content/tree/master/languages/ruby).

![](./Fedora_developer_portal_ruby.png)

## Testing instance on OpenShift

Nowadays the portal is hosted on Openshift instance here [https://developer-phracek.rhcloud.com/](https://developer-phracek.rhcloud.com/), but it wasn't officialy released as was mentioned above. For better orientation for all users the portal should have reference directly on [http://getfedora.org](http://getfedora.org).

This is good place to say thank you to Adam Šamalík, who is co-maintainer of the Fedora Developer Portal.

**References:**

*   [https://github.com/developer-portal/content](https://github.com/developer-portal/content)
*   [https://fedoraproject.org/wiki/Websites/Developer](https://fedoraproject.org/wiki/Websites/Developer)
*   [https://developer-phracek.rhcloud.com/](https://developer-phracek.rhcloud.com/)
*   [https://en.wikipedia.org/wiki/Markdown](https://en.wikipedia.org/wiki/Markdown)
*   [http://blog.samalik.com/fedora-developer-portal/](http://blog.samalik.com/fedora-developer-portal/)
*   [http://blog.samalik.com/fedora-developer-portal-prototype/](http://blog.samalik.com/fedora-developer-portal-prototype/)
*   [http://taiga.cloud.fedoraproject.org/project/fedora-developer-portal/kanban](http://taiga.cloud.fedoraproject.org/project/fedora-developer-portal/kanban)
