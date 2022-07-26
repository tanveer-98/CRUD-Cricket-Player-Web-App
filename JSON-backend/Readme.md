Step 1 ---- Create a folder
Step 2 ------ npm init
Step 3 ------ npm install json-server --save
Step 4 ------ create server.json file
Step 5 ------ Paste the below code
 
 
{
    "players": [
        {
            "id": "1",
            "name": "Dhawan",
            "category": "Batsman",
            "country": "India",
            "image": "https://www.cricbuzz.com/a/img/v1/152x152/i1/c170660/shikhar-dhawan.jpg"
        },
        {
            "id": "2",
            "name": "Dhoni",
            "category": "Keeper Batsman",
            "country": "India",
            "image": "https://www.cricbuzz.com/a/img/v1/152x152/i1/c170677/ms-dhoni.jpg"
        },
        {
            "id": "3",
            "name": "Virat",
            "category": "Batsman",
            "country": "India",
            "image": "https://www.cricbuzz.com/a/img/v1/152x152/i1/c170661/virat-kohli.jpg"
        }
    ]
}
 
 
Step 6 ------ Go to package.json
Step 7 ------ Paste the below code
 
"scripts": {
    "start": "json-server -p 3006 -w server.json"
},
 
Step 8 ----- npm start
Step 9 ----- type http://localhost:3006/players
Step 10 ----- add http://localhost:3006 as baseUrl in your service/index.js