---
layout: post
title:      "Rails Project - Final Thoughts"
date:       2020-08-02 03:30:23 +0000
permalink:  rails_project_-_final_thoughts
---


Ruby on Rails is surely a magical thing. So many behind the scene actions that you just got to trust what is happning, and understand how it affects your code. I decided to build my app for dogs, because I love dogs and I have a dog. The app is called Sniff n Play, because the idea was it being a social/dating app for dogs. 


I think the hardest thing for me while building this app was the ActiveRecord Associations. First, the idea to come up with a has_many through: association was already taking up a lot of time. Oh and don't even get me started on time. Two weeks to build what the instructor says to be the hardest project doesn't make sense to me. But, life isn't always fair and it is what it is. Anyways, it is very crucial to have your tables and models set up logically and in a flowy manner. Half the battle of setting up your application is understanding what your data relationships will look like. By setting up your data relationships, you'll be bale to retrieve data about all the objects that are associated with another. For instance, If you want to see all the comments one of your users left on another user's timelines, we can build this functionality out due to ActiveRecord. 

Rails supports six types of associations:

belongs_to
has_one
has_many
has_many :through
has_one :through
has_and_belongs_to_many

When you create an association, Rails makes two major assumptions – first, that the class of the model your association points to is based directly off of the name of the association, and, second, that the foreign key in any belongs_to relationship will be called yourassociationname_id. Any time you go away from these defaults, you just need to let Rails know what kind of class to look for and which foreign key to use.

To sum up what I've learned about associations, and Active Record, is that, no matter how complex our associations are, Active Record is really good at managing that complexity for us. We can always drop down a level of abstraction if needed to customize the way our application behaves.


