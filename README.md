# mSchool Curriculum

mSchool was an e-learning app created by Sam Bhattacharyya, Tunde Alawode and Thomas Richman in 2016, with ~2000 videos targetting the West African WAEC secondary curriculum, to help students supplement their classes with Khan-Academy style video lessons, recorded in an ultra data-light format (~10kbps)


# Curriculum Data

The curriculum data is stored in a single JSON file in curriculum.zip.

The curriculum is broken down into several courses (Math, Physics, Chemistry, Economics and Biology).

Courses are further broken down into: Sections > Subsections -> Lessons -> Videos, which is all stored within JSON file.

Videos are the lowest subunit, and just have an ID assocated with it.

# Videos

The videos themselves are compiled in our own ".lrn" format. They can be played back with a Javascript player (see demo folder)*[]:

The LRN files themselves are stored on AWS S3. The API for accessing a given video is

https://s3-eu-west-1.amazonaws.com/dotlearn-io-dist/[video-id]/amr_nb5.lrn


# Player

You can see an example of the player in the demo folder. The UI is a bit ugly, and was built in 2015. The source code from the player is [here](https://github.com/Vectorly/mschool-player).



