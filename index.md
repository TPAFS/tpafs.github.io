This repository serves as a landing page from which one can navigate all of the public
repositories and static sites maintained by Persius on Github.


We currently maintain the following public repositories:

{% for repository in site.github.public_repositories %}
- [{{ repository.name }}]({{ repository.html_url }})

    {{repository.description}}
{% endfor %}