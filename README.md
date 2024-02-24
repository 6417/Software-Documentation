# 6417 Dokumentation

## How to run the documentation
### Running the website
To run the website, just start the docker container and connect to it
```sh
docker compose up --build -d
```
Then, after starting, connect to http://localhost:8000
### Stopping the webserver
To stop the webserver, stop the compose stack
```sh
docker compose down
```

## Contributing to the docs
To contribute the repo, visit the 
[mkdocs guide](https://www.mkdocs.org/user-guide/writing-your-docs/) for writing docs
### In short
- To add a page to the nav, link it in mkdocs.yaml
- To link to a page from within the page, create it as markdown and link to it from a page
