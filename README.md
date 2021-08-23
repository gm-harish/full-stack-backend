# full-stack-backend


It is the production ready file, the server serves both front end and backend.

app.use(express.static(path.join(__dirname, '/build')));, it is used to load statis files like images etc.


app.get('*', (req, res) => {
    res.sendFile(path.join(__dirname + '/build/index.html'));
});
it is used to serve the frontend whenever some users hits the server. It is used for both frontend and requesting data from api's. (backend).

We can directly deploy in aws.

we can use postman to check the api.
