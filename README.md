# unoconv-api

# Build - exemple

docker build -t convert:v1 .

# Run - exemple

```sh
$ docker run -d -p 8080:3000 convert:v1
```

# Usage

Post the file you want to convert to the server and get the converted file in return.

See all possible conversions on the [unoconv website](http://dag.wiee.rs/home-made/unoconv/).

The API for the webservice is /unoconv/{format-to-convert-to} so a docx to pdf conversion would be:

```sh
$ curl --form file=@myfile.docx http://192.168.0.111/convertPDF/pdf > myfile.pdf
```
