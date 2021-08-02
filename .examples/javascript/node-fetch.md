### GET
```javascript
 fetch('https://azrael.gg/api/v2/get/641795527444529152', {
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
const body = { id: '641795527444529152', reason: 1, proof: 'https://cdn.azrael.gg' };

fetch('https://azrael.gg/api/v2/add', {
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
const body = { id: '641795527444529152', type: 'Notes', value: 'There are no notes' };

fetch('https://azrael.gg/api/v2/edit', {
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
 fetch('https://azrael.gg/api/v2/delete/641795527444529152', {
         method: 'DELETE',
         headers: {
             'Authorization': 'Your Bearer Token',
             'Content-Type': 'application/json'
         },
     })
     .then(res => res.json())
     .then(json => console.log(json));
```