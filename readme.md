# Live-Docker

> Repositório criado para aprender sobre docker referente à live https://www.youtube.com/watch?v=yb2udL9GG2U

COPY . .
=> Copiando todos os arquivos da pasta que está o dockerfile e colando dentro da imagem. Ou seja, quando for rodar esse dockerfile, ele vai pegar os arquivos que estão ali e jogar dentro daquela imagem

RUN go build main.go
=> Vai gerar o executável

EXPOSE 8080
=> Se algum outro container quiser falar com ele, ele vai responder na porta 8080

ENTRYPOINT ["/.main"]
=> Quando o container for rodar eu quero que voce execute o arquivo main

-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-= <br/>
docker build -t go-live-fullcycle .<br/>
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-= <br/>
o -t é para 'taguear' a imagem, ou seja, apelidar