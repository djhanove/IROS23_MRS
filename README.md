# IROS23_MRS_Workshop

Followed the this guide on how to enable github pages: [youtube](https://www.youtube.com/watch?v=owHfKAbJ6_M&t=111s)

1. Make a new repo
2. Go to settings
3. Enable Github pages
4. Clone repo
5. Open VSCode with repo folder
6. Install Docker and Dev Containers extension for VSCode
7. Fetch Jekyll container image: [this one](https://hub.docker.com/r/jekyll/jekyll/)
8. hit ctrl + shift + p, "open folder in container" to open the repo folder within the docker container
9.`jekyll` in VSCode terminal (ctrl + shift + s to create new VSCode terminal)
10. ``` bundle init
	bundle add jekyll --version "~>3.9.0"
	bundle exec jekyll new --force --skip-bundle .
	bundle add webrick
	bundle install
	bundle update
	bundle exec jekyll serve --livereload

The last command will automatically render any changes to the website on your localhost

11. Copy the url from the gitpages into baseurl and url field in _config.yml
`baseurl: "/IROS23_MRS_Workshop"`
`url: "https://uzh-rpg.github.io"`
12. In Gemfile, we need to uncomment the gem line with "github-pages"
13. This website uses the bluma clean theme [repo](https://github.com/chrisrhymes/bulma-clean-theme/). Example website is [here](https://www.csrhymes.com/bulma-clean-theme/)

