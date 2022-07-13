Part 1:
https://swapi.dev/api/people/4 "height" : "202"
https://swapi.dev/api/planets/2  "population": "2000000000"
https://swapi.dev/api/starships/10   "manufacturer": "Corellian Engineering Corporation",
https://swapi.dev/api/people/2, https://swapi.dev/api/species/2  "name": "Droid"
"films": [
        "https://swapi.dev/api/films/1/", "title": "A New Hope",
        "https://swapi.dev/api/films/2/",   "title": "The Empire Strikes Back",
        "https://swapi.dev/api/films/3/", "title": "Return of the Jedi",
        "https://swapi.dev/api/films/4/", "title": "The Phantom Menace",
        "https://swapi.dev/api/films/5/", "title": "Attack of the Clones",
        "https://swapi.dev/api/films/6/"  "title": "Revenge of the Sith",
    ],
https://swapi.dev/api/starships/?search=falcon 

Part 2: 
POST request accepts a body, and its expecting a text Key. 
GET request return's an array of an object data type.
https://practiceapi.devmountain.com/api/posts/?id=555
Request query is missing required text property. code 409
https://practiceapi.devmountain.com/api/posts   
    {
       "id": 74,
        "text": "sana",
        "date": "13 Jul 2022"
    }
https://practiceapi.devmountain.com/api/posts/?id=74
  {
        "id": 74,
        "text": "blue",
        "date": "13 Jul 2022"
    }
    https://practiceapi.devmountain.com/api/posts/filter/?text=blue
    application/json; charset=utf-8
    409 
Request was missing req.query.id or req.body.text
 
 You get all the posts, because it doesn’t let you filter by id. 
