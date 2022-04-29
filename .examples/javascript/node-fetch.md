### GET
```javascript
 fetch('https://api.azrael.gg/v5/get/933402903937437696', {
         method: 'GET',
         headers: {
             'Authorization': 'Your Bearer Token',
             'Content-Type': 'application/json'
         },
     })
     .then(res => res.json())
     .then(json => console.log(json));
```
### POST
```javascript
const body = { id: '933402903937437696', reason: 1, proof: 'https://cdn.azrael.gg' };

fetch('https://api.azrael.gg/v5/bans/add', {
        method: 'POST',
        body: JSON.stringify(body),
        headers: {
            'Authorization': 'Your Bearer Token'
            'Content-Type': 'application/json'
        },
    })
    .then(res => res.json())
    .then(json => console.log(json));
```
### PATCH
```javascript
const body = { id: '933402903937437696', type: 'Notes', value: 'There are no notes' };

fetch('https://api.azrael.gg/v5/edit', {
        method: 'PATCH',
        body: JSON.stringify(body),
        headers: {
            'Authorization': 'Your Bearer Token'
            'Content-Type': 'application/json'
        },
    })
    .then(res => res.json())
    .then(json => console.log(json));
```
### DELETE
```javascript
 fetch('https://api.azrael.gg/v5/delete/933402903937437696', {
         method: 'DELETE',
         headers: {
             'Authorization': 'Your Bearer Token',
             'Content-Type': 'application/json'
         },
     })
     .then(res => res.json())
     .then(json => console.log(json));
```
