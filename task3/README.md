#### Build Backend
`docker build -f ./back-end/Dockerfile -t task3-back ./back-end`

#### Run Backend
`docker run -p 5252:5252 -it task3-back`

#### Build FrontEnd
`docker build -f ./front-end/Dockerfile -t task3-front ./front-end`

#### Run FrontEnd
`docker run -p 9000:9000 -it task3-front`
