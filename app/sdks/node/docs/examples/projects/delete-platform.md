const sdk = require('node-appwrite');

// Init SDK
let client = new Projects.Client();

let projects = new sdk.Projects(client);

client
    .setProject('')
    .setKey('')
;

let promise = projects.deletePlatform('[PROJECT_ID]', '[PLATFORM_ID]');

promise.then(function (response) {
    console.log(response);
}, function (error) {
    console.log(error);
});