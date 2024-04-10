### Setting up the backend
1. Install the dependencies using pip 
    ```
        pip install -r requirements.txt
    ```
### Starting Fast API backend
Starting backend for development :
```
    python app.py -e dev 
```
Starting backend for production :
```
    python app.py -w 4
```
Visit [http://localhost:8000/hello](http://localhost:8000/hello) to check if backend api running properly. You should see this message :
```json
    {
        "message": "Hello from book-recommender-api"
    }
```
API docs will be available at :
- [http://localhost:8000/docs](http://localhost:8000/docs)
- [http://localhost:8000/redoc](http://localhost:8000/redoc)

## To work on UI (React)
### To start the development server (vite + react + tailwindcss) :
```
    cd ui
```
If you're running it for the first time :
```
    npm i
```
then
```
    npm run dev
```
### Building the ui
```
    npm run build 
```
The output directory will be : [/public](public)

## Other important stuff
- To change backend port in development or production use [/config](config).
- [Dataset](data) taken from [kaggle](https://www.kaggle.com/datasets/arashnic/book-recommendation-dataset).
- Followed tutorial of [CampusX](https://www.youtube.com/watch?v=1YoD0fg3_EM&t=2437s) to create this project's backend.
