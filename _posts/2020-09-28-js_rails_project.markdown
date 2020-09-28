---
layout: post
title:      "JS/Rails Project"
date:       2020-09-28 21:40:01 +0000
permalink:  js_rails_project
---

For my fourth project, I decided to build an exercise tracker application, where users can track/log their exercises. The frontend is built with HTML, CSS and Vanilla JS, all the while communicating with my backend API that I built with Ruby and Rails. 

This was a very fun project for me because it tested my knowledge in all area of web development, from styling to html to JS and Rails. I wanted to build an exercise tracker because I like to try to stay healthy and active, and also because in general I like to track everything I do, and see my progress. Like with all projects, the first thing to do is plan and draw out the direction you want to take your app. First is to set up my backend. I generated a new RAILS API using `rails new <my_app_name> --database=postgresql --api.` I made sure to attach the --api flag so rails knows to remove many of the default features and middleware, mostly related to the browser. Controllers will inherit from `ActionController::API `rather than `ActionController::Base` and generators will skip generating views. Next, I created my models, controllers, and migrations. One thing different than the previous project is the introduction to CORS, which stands for Cross-Origin Resource Sharing. The purpose of CORS is to prevent scripts like `fetch()` from one origin accessing a resource from a different origin unless that resource specifically states that it expects to share. To ensure CORS works, I need to download the gem and uncomment some lines in the config/initializers/cors.rb file. Another new concept in the backend is serializers. There are a couple serializer gems to use. I decided to use the fast jsonapi one. Serialization is the process of translating a data structure or object state into a format that can be stored. 

In my frontend, I created an exercise.js file, index.js file, and index.html file. The main getaway with the .html file is to be sure to connect it to my index and exercise .js files through script tags (`<script type="text/javascript" src="index.js"></script>`). When it came to building out my fetch calls, I found myself having the most difficulty with calling my delete function. The challenge with this was grabbing the id of that specific exercise, and deleting that specific object. 


function removeExercise(e) {
    e.preventDefault();
    let execId = e.target.id[3];
    fetch(`http://localhost:3000/api/v1/exercises/${e.target.id}`, {
        method: "DELETE",
        headers: {
            "Content-Type": "application/json",
            "Accept": "application/json"
        }
    })
    .then(function(resp){
        if (resp.status == 204)
            location.reload();
        else
            throw new Error(resp.message)
            console.log(resp.status)
    })
    .catch(error => {
        alert('FAIL. TRY AGAIN');
    });
}
        alert('FAIL. TRY AGAIN');
    });
}






