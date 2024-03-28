
# HelloWorld LMS

This is a project designed to make Education and Job opportunities easily accessible in one platform.

## Features

### Courses

The Platform offers a variety of courses, which are pre-recorded by instructors and posted on the website. The courses that a student is enrolled in or that the instructor has posted appear in their respective dashboards.
### Assignments & Quizzes

The platform allows instructors to add assessments that in turn the students attempt and get feedback on their grades. This allows to track user progress.
### Job Matching

The platform allows admins to post jobs on the platform highlighting the skills needed and automatically all the students who possess the skills specified and are enrolled in a course that offers those skills are sent emails automatically.
````
Node JS

const relevantCourses = await Course.find({
      category: { $in: requiredSkills },
    }).select("_id");

    const relevantCoursesId = relevantCourses.map((course) => course._id);

    // Find matching users
    const matchingUsers = await User.find({
      skills: { $in: requiredSkills },
      courses: { $in: relevantCoursesId },
    });
````

### User Profile Management
The Platform allows users to update their profiles allowing them to put their skills and interests hence allowing them to have access to Job opportunities. This section also allows admins to remove or grant access to instructors on the platform.


## Usage

- Clone this repository `https://github.com/GasanaJr/hello-world-frontendV1.1.git`.
- Change the working directory `cd hello-world-frontendV1.1`.
- Open `index.html` in your favorite browser.


### Alternatively
- Visit the hosted fronted application at [HelloWorld](https://helloworldprojectv1.netlify.app/)
- Visit the hosted backend at [HelloWorld Backend](https://hello-world-backend-0jav.onrender.com)

## Accounts

- Student: Email: `gasana@maicoltd.com` Password: `Hello@123`
- Instructor: Email: `instructor@helloworld.com` Password: `Hello@123`
- Admin: Email: `admin@helloworld.com` Password: `Hello@123`

## Tech Stack
- HTML
- CSS
- Javascript
- Node Js

## Acknowledgements

- [How to write a Good readme](https://bulldogjob.com/news/449-how-to-write-a-good-readme-for-your-github-project)

- [Design Inspired By Code With Sadee](https://github.com/codewithsadee)

## Authors

- [@Didas Junior](https://www.github.com/GasanaJr)


