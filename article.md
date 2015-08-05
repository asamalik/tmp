# Fedora developer portal

Fedora developer portal has arised as an idea from Josef Stribny and Petr Hracek. The aim of the portal is to give an overview about important development tools and projects in Fedora. Focus is targeted on beginners, advanced users and developers.   
You may as a question: why do we need that portal?  
The answer is really simple: In order to make it easy for developers to develop applications on Fedora - which might be Fedora Workstation, Server or Cloud - we want to show them how to use Fedora easily and provide them with best practises. If we are able to cover a set of areas, then using Fedora will become a pleasant experience for users and developers.

## Who will use the portal?

Fedora Developer Portal would show users how to develop on Fedora easily, and introduces them to new projects and tools that are available in Fedora. Fedora users will have an overview about:

*   new technologies
*   available developer languages
*   projects released in each Fedora release cycle
*   important tools in Fedora (like Docker, Vagrant, DevAssistant etc.)
*   other tools which can be used for development

The portal should be of course used by users which would like to develop applications on Fedora. Each section would provide a guide on how to setup an environment or system for given use-case.

Nowadays, the portal looks like this: [https://developer-phracek.rhcloud.com/](https://developer-phracek.rhcloud.com/). However, the portal is still under development -so the design of pages is going to change.

![](./Fedora_developer_portal_main.png)

How the Powerful Tools section looks like can be seen on the following picture or here: [https://developer-phracek.rhcloud.com/tools.html](https://developer-phracek.rhcloud.com/tools.html).

![](./Fedora_developer_portal_tools.png)

## How to write a content for specific area?

It is needed to cover all parts with guides in order to provide enough information about developement in Fedora. How to create a given area is described below.

The whole portal content is placed in a GitHub repository [https://github.com/developer-portal/content](https://github.com/developer-portal/content). If you want to contribute, you need to _fork_ our GitHub repository and make a pull request. To make changes, you can either clone the repository to your system or use the web interface directly.

### How to clone the repository

To clone your repo, use the following command:

git clone git@github.com:{your_github_name}/content.git
  
### How to write a content directly on the GitHub website

Select a part which you would like to create, e.g. nodejs [https://github.com/developer-portal/content/tree/master/tech/languages/nodejs](https://github.com/developer-portal/content/tree/master/tech/languages/nodejs).

*   Click on **+** (which is mentioned after nodejs) to create a new file and write down a name of the file
*   Provide a content.
*   When the content is finished, press the "Propose a new file" button to save the file to GitHub
*   Click on the "Pull Request" button and write a comment about it.

Next step is on Fedora Developer Portal team to review it and give you a feedback.

### How to cover specific area?

Each section must begin with mark in configuration language YAML, which says where relevant area belongs to. For main page **ruby** it is e.g.:

<pre>  ---
  title: Ruby
  page: ruby
  section: tech-languages
  ---
  </pre>

Each page, except main page, should have syntax like:

<pre>  ---
  title: Some another text which belongs to ruby
  page: ruby
  ---
  </pre>

The content itself is written in a [MarkDown](https://en.wikipedia.org/wiki/Markdown) language.

### What is missing nowadays

Fedora Developer portal does not have following parts:

*   Tools - DevAssistant, Docker, Vagrant
*   Programming languages - Python, Php, Perl, Go, C, NodeJS, Java
*   databases - PostgreSQL, MariaDB, SQLite
*   Deployment - Copr, SCL, Nulecule, xdgapp, rolekit, openshift
*   Fedora Next

Parts which doesn't have a content can be found on GitHub here [https://github.com/developer-portal/content/issues](https://github.com/developer-portal/content/issues).

### How to publish your content?

If you cover a part of content, you should crate a Pull Request. It will be then reviewed by the the portal developers and other community members that give you a feedback. You can then collaborate with others on your content.

### Ruby example on the portal

As a example, have a look at the Ruby content, which is already available on portal [https://github.com/developer-portal/content/tree/master/languages/ruby](https://github.com/developer-portal/content/tree/master/languages/ruby).

![](./Fedora_developer_portal_ruby.png)

## Testing instance on OpenShift

The developer instance of the portal is hosted on Openshift here [https://developer-phracek.rhcloud.com/](https://developer-phracek.rhcloud.com/), but it wasn't officialy released - it is a development instance. For better orientation for all users the portal should have a reference directly to [http://getfedora.org](http://getfedora.org).

This is good place to say thank you to Adam Šamalík, who is co-maintainer of the Fedora Developer Portal.

**References:**

*   [https://github.com/developer-portal/content](https://github.com/developer-portal/content)
*   [https://fedoraproject.org/wiki/Websites/Developer](https://fedoraproject.org/wiki/Websites/Developer)
*   [https://developer-phracek.rhcloud.com/](https://developer-phracek.rhcloud.com/)
*   [https://en.wikipedia.org/wiki/Markdown](https://en.wikipedia.org/wiki/Markdown)
*   [http://blog.samalik.com/fedora-developer-portal/](http://blog.samalik.com/fedora-developer-portal/)
*   [http://blog.samalik.com/fedora-developer-portal-prototype/](http://blog.samalik.com/fedora-developer-portal-prototype/)
*   [http://taiga.cloud.fedoraproject.org/project/fedora-developer-portal/kanban](http://taiga.cloud.fedoraproject.org/project/fedora-developer-portal/kanban)
