# Model Inference Server (Hurricane Harvey Neural Networks)

Part 3: 
Docker image link: 
https://hub.docker.com/r/ayushisapru02/inference_server

Instructions:

Pull the Docker image (hosted on Docker Hub) using: 
docker pull ayushisapru02/inference_server:latest

Start server:
docker compose up

Stop server: 
docker compose down

Example requests:
GET model summary: 
curl http://localhost:5000/summary

POST inference request:
curl -X POST -F image=@path/to/image.jpg http://localhost:5000/inference
