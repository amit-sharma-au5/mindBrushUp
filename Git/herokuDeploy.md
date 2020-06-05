# MERN App Deployment in Heroku

### First check PORT and add process.env.PORT

### Create custom  variable 
```javascript 
    if(process.env.Node_ENV === 'production'){
        app.use(express.static('../frontend/build'))
    }

```