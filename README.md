# Stanford CoreNLP Web API Server

This is a Docker container for running the [Web API Server](https://stanfordnlp.github.io/CoreNLP/corenlp-server.html) for [Stanford CoreNLP](https://stanfordnlp.github.io/CoreNLP/index.html).

See: https://hub.docker.com/r/joeworks/corenlp-server/

## Usage
```bash
docker run --name corenlp -p 9000:9000 -d joeworks/corenlp-server
``` 

## Support for other language model
By default the 'english' [language model](https://stanfordnlp.github.io/CoreNLP/download.html) is included. If you wish to add another supported languages, add `-e "LANGUAGE=language-name"`, for example to include the 'chinese' language model:
```bash
docker run --name corenlp -p 9000:9000 -d -e "LANGUAGE=chinese" joeworks/corenlp-server
``` 
