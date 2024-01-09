# Product app backend
export PORT=4040
export MONGODB_URI="mongodb+srv://someusername:somepassword@cluster100.rq134334.mongodb.net/product?retryWrites=true&w=majority"

````console
//clone repository with --bare
git clone https://github.com/zeeemughal/product_backend.git 

// create a new repository and push to that
git remote set-url origin git@github.com:faisalabbasm/product-backend-v2.git

//push to new remove
git push -u origin main


````

````console
// create docker file

//build docker file
docker build -t faisalabbasm/product-backend-v2:1.0 .

// run docker image
docker run -e PORT=4040 -e MONGODB_URI="mongodb+srv://evently_user:BpNf2C0bFx09vDKD@evently.ugjztes.mongodb.net/?retryWrites=true&w=majority" -p 4040:4040 -d faisalabbasm/product-backend-v2:1.0
	
//push to docker registry
docker push faisalabbasm/product-backend-v2:1.0
````