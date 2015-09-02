# Rails-Interview

Ruby Programming Questions 

1. Write a program to find the sum of all numbers in an array.

2. ["TEST", "BEST", "TRUST"] . Write a program which receives an array input, validates the input and returns a hash with count of alphabets "T" and "E"

3. Convert a = [["row", 3], ["your", 1], ["boat", 1]] to ["row", "row", "row", "your", "boat"]. The first element in the nested arrays is the word that should be displayed and the second element in the nested array is the number of times the word should be displayed.

3.1 Given an array of positive integers, write a function which returns all the unique pairs which add (equal) up to 100.

Example data:

sample_data = [0, 1, 100, 99, 0, 10, 90, 30, 55, 33, 55, 75, 50, 51, 49, 50, 51, 49, 51]
sample_output = [[1,99], [0,100], [10,90], [51,49], [50,50]]

  
4. Take Home assignment

	2.David Heinemeier Hansson's github url is https://github.com/dhh .

	Github provides information about his public commits in JSON format at https://api.github.com/users/dhh/events/public .

	In the JSON data there is an attribute called "type" which denotes what kind of commit it was.

	Let's say that we give following score to DHH based on the "type" of the commit

	IssuesEvent = 7
	IssueCommentEvent = 6
	PushEvent = 5
	PullRequestReviewCommentEvent = 4
	WatchEvent = 3
	CreateEvent = 2
	Any other event = 1
	Task

	Write a ruby program which when executed prints the score of https://github.com/dhh . The answer printed on the terminal should be like this.

	Calculate the score based on the item results returned only from first page of that API call. Do not worry about pagination.

	$ ruby exercise.rb
	DHH's github score is xxx


1. What is rack in rails ? What is its advantage ?

2. What’s the issue with the controller code below? How would you fix it?
	class CommentsController < ApplicationController
	  def users_comments
	    posts = Post.all
	    comments = posts.map(&:comments).flatten
	    @user_comments = comments.select do |comment|
	      comment.author.username == params[:username]
	    end
	  end
	end

3. Is http a stateless protocol ? How does sessions work in Rails ?

4. Product and Vendors are in many to many association. Vendor has a name
   Product has different prices for different Vendors
   Model this problem and write an instance method for Vendor  named "costly_product" to 
   find the product with the largest price for any vendor. 

5. What is russian doll caching ?

6. What are strong parameters and what is the requirement for the same ?

7. How to write an AJAX function that checks if request is AJAX request and if true then sends out JSON response containing a partial file as well as a message about response "success" or "fail".

8. Explain polymorphic association with example.

9. Switch database connection for a purticular model.

10. State based system for orders - How to manage inside a wizard.

Q1. Space Rockets are dangerous. SpaceX has decided to give you a free ride on their new RuberX autonomous space rocket to the international space station. The only catch is that the code for RuberX is written entirely in Ruby. Would you take the ride? Give at least 3 reasons why you would, 3 reasons why you wouldn’t

# 1. Maintainable
# 2. Conventional
# 3. Clean 
#
# 1. Partially Compiled 
# 2. 
# 3.



Q2. What is Session and Cookies? When is it best to use one over the other



Q3. What do the following two variables tell you about themselves?

1. @@foobar
2. $foobar






Q4. What is Eager loading? /N + 1 queries problem
What is the difference between the following:
   ——>includes
   ——>preload
   ——>Joins
   
   
   
   
   
 Q5. Choosing Between has_many :through and has_and_belongs_to_many? Where to use which one?




Q6 Polymorphic Associations ? How do you set them up ? Why do we use them?


class Product
end

class Vendor
end




Q7. Finding by SQL? Would you ever need to use this in your code. If yes them why?


Q8. How would you debug an error on a rails application
