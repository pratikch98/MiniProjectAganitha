# MiniProjectAganitha

ssh MiniProject@20.193.238.210 // connecting to the ubuntu server ( on azure)

sudo apt install apt-transport-https ca-certificates curl software-properties-common     //installing docker
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu `lsb_release -cs` test"
sudo apt update
sudo apt install docker-ce

docker pull postgres //docker container for postgresql
docker run --name postgres0 -e POSTGRES_PASSWORD=mysecretpassword -d -p 5432:5432 postgres //start postgres on port 5432

sudo docker run -p 8888:8888 jupyter/scipy-notebook:33add21fab64 //install docker container jupyter, start at port 8888

![azure_vm](https://user-images.githubusercontent.com/96818440/147661665-7f6d609d-d588-4d31-9149-b6ee166b84c3.PNG)  (azure vmware for ubuntu)
![Capture](https://user-images.githubusercontent.com/96818440/147661872-e51bbfb4-e771-40a6-916b-bec0c7d45e5a.PNG)   (jupyter notebook) 

![postgres](https://user-images.githubusercontent.com/96818440/147662634-a1f083ed-4677-4e6b-b015-855132087e4b.PNG) (postgres table, contains no data)
