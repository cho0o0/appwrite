const sdk = require('node-appwrite');

// Init SDK
let client = new Projects.Client();

let projects = new sdk.Projects(client);

client
    .setProject('')
    .setKey('')
;

let promise = projects.createKey('[PROJECT_ID]', '[NAME]', []);

promise.then(function (response) {
    console.log(response);
}, function (error) {
    console.log(error);
});