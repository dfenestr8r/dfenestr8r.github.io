# dfenestr8r.github.io

## Projects
### [Contact Service Application Enhancement](https://github.com/dfenestr8r/dfenestr8r.github.io/blob/main/cs320MobileApp.zip)

#### Description

Originally created as a suite of Java classes and JUnit test classes in CS-320 to perform basic tasks for a mobile application, I extended the
data structure to demonstrate the efficiency of a hashmap over an ArrayList for CRUD operations in large datasets.

#### Narrative for Algorithms and Data Structures

This is the ContactService module from CS320, built as part of a mobile app backend. It consists of the Contact data class and a ContactService that manages a collection of contacts supporting add, delete, update, and lookup operations. It was originally created during CS320 and uses a HashMap as its backing data structure. I added ContactServiceArrayList as an alternate implementation and a benchmark test class to compare the efficiency of CRUD operations between the two. The specific components that showcase algorithms and data structures knowledge are understanding that HashMap provides O(1) average-case lookup via hashing while ArrayList requires O(n) linear scan, implementing the same interface with both structures so the comparison is fair, and using worst-case targeting in the benchmark (looking up the last element forces ArrayList to scan the entire list). 
	I believe the enhancements are in line with course outcomes three and four (Design and evaluate computing solutions that solve a given problem using algorithmic principles and computer science practices and standards appropriate to its solution, while managing the trade-offs involved in design choices (data structures and algorithms), Demonstrate an ability to use well-founded and innovative techniques, skills, and tools in computing practices for the purpose of implementing computer solutions that deliver value and accomplish industry-specific goals (software engineering/design/database))

Just like with the previous enhancement, the real challenge was reinstalling and reconfiguring the Eclipse workspace to properly run the tests like I had in CS-320, but once all of that was ironed out, the main challenges were properly implementing the ArrayList test class and creating meaningful benchmarks to compare it against the hashmap implementation.


[Download Link](https://github.com/dfenestr8r/dfenestr8r.github.io/blob/main/cs320MobileApp.zip)



### [Weight Tracker Mobile App](https://github.com/dfenestr8r/dfenestr8r.github.io/blob/main/WeightTrackerEnhanced.zip)

#### Description

Originally created as a skeleton Android app with basic user authentication, SQLite database schema, and UI, I enhanced the front and back-end
to turn it into a fully fleshed out and usable weight tracking app.

#### Narrative for Software Design and Engineering

This artifact is from CS-360, Mobile Architecture and Design, which was a course I took about six months ago. It's an Android app that is meant to help users track their weight against a set goal weight. At the end of the course, the app I submitted was technically complete with database integration, a login screen, and SMS notifications, but it didn't demonstrate any knowledge of UX design, realistic software requirements, or modern Android design language.
I selected this artifact for a couple of reasons. The first is that it had a lot of room for improvement. The UI was ugly and didn't properly fit any screens I tested on, some basic features were broken, and the use cases it was designed for were unrealistic. Another reason I selected it is that the backend was actually in a pretty good place. The SQLite server worked well and the structure of the application was in place, so it seemed like a good candidate to focus on majorly improving the design elements and refining the engineering aspects that were already present. As of this submission, the UI has been overhauled using Android Material Design 3, including an improved color theme, improved visual consistency and screen spacing, and more intuitive layout. Existing issues including the "Set Goal" button not functioning have been fixed through changes to the database and dashboard helper methods. When a user adds a weight, it displays the distance from their goal weight on that entry (e.g., +20 or -10 pounds from their goal). There are more enhancements planned, but I feel that these changes demonstrate the third a fourth course outcomes ("Design and evaluate computing solutions that solve a given problem using algorithmic principles and computer science practices and standards appropriate to its solution, while managing the trade-offs involved in design choices (data structures and algorithms)", and "Demonstrate an ability to use well-founded and innovative techniques, skills, and tools in computing practices for the purpose of implementing computer solutions that deliver value and accomplish industry-specific goals (software engineering/design/database)").
The changes I have made so far are mostly minor and more enhancements are planned for the final submission. The biggest obstacle to making these changes was the fact that I'm using a different PC than I was using when I first developed the app, so I had to go through a lot of troubleshooting to get the Android Studio environment to a place where it would work properly with the existing codebase and then make the updates I needed for the UI and database enhancements. New features are planned to demonstrate an improved understanding of software design and technical skills. Troubleshooting the issue with the "Set Goal" button took a lot of time due to my lack of Android development experience, but once I found the root issue the fix was easy. Overhauling the UI was also a tedious process, but using a more modern toolkit makes the app more maintainable and future updates will be much easier. Adding the new "distance from goal weight" feature was very simple and mostly included to make sure that this submission wasn't only focused on bug fixes and UI updates.

#### Narrative for Databases

The artifact chosen is the WeightTracker Android app developed in CS-360. It is intended to provide users with an easy way to track their weight changes against a set goal. I had already made changes to the UI, added new features, and fixed several bugs for a previous milestone, but these edits focus on the backend to demonstrate knowledge of databases. The original plan was to compute moving 7- and 30-day averages directly in SQL, but it was more easily done directly with Java and lines up better with the purpose of the app. I went with the simpler solution and implemented the Statistics screen, but also made changes to the backend logic to use structured db.query() calls instead of a previous rawQuery in the getAllWeights method and take the userId parameter filtered with a WHERE user_id=? Clause. 
	Although this enhancement didn’t involve as much tinkering with the database as I was intending it to, I still feel it is a good enough enhancement to the original app to be worth submitting for the database category. At this point, every aspect of this app has been improved and I’m happy with the foundation of it.
	The biggest challenge for this set of enhancements was trying to force my original idea of moving averages directly in SQL, which would have been doable but wouldn’t have improved the user experience of the app itself and would have been useless in practice. Once I decided to go through in the direction that would actually improve the software as a whole, the challenges were mostly layout constraints, adding the ViewHolder class, and properly using index math to build the Statistics page. Catching the bug in the database with the getAllWeights method would have been difficult to find without real multi-user data




[Download Link](https://github.com/dfenestr8r/dfenestr8r.github.io/blob/main/WeightTrackerEnhanced.zip)



