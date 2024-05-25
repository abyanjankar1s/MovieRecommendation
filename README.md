# MovieRecommendation
Object Oriented Programming: Designing Movie Recommendation. 




# DEMO

      user1 = User(123, 'Luka')
      user2 = User(231, 'Kyrie')
      user3 = User(222, 'Lively')
      
      movie1 = Movie(1, 'Inception')
      movie2 = Movie(2, 'Seven')
      movie3 = Movie(3, 'Dark Knight')
      
      ratings = RatingRegister()
      ratings.addRating(user1, movie1, MovieRating.FIVE)
      ratings.addRating(user2, movie2, MovieRating.FOUR)
      ratings.addRating(user1, movie2, MovieRating.ONE)
      ratings.addRating(user2, movie3, MovieRating.THREE)
      
      recommender = MovieRecommendation(ratings)
      
      print(user1._name +" is recommended " + recommender.recommendMovie(user1))
      print(user2._name +" is recommended " + recommender.recommendMovie(user2))
      print(user3._name +" is recommended " + recommender.recommendMovie(user3))
      
      aayushbyanjankar@Aayushs-MacBook-Air MovieRecommendation % python3 movie.py
      Luka is recommended Dark Knight
      Kyrie is recommended Inception
      Lively is recommended Inception
