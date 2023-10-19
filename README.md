# LearningCenterCore

This is the initial tutorial site for Vorakor Technologies Learning Center, though there may be some other code coming in later.

## Technical Stack

The initial focus of this project is speed. To that end, I will choose a stack I am more comfortable with and implement that stack to get this up and running faster, and to deploy to a live server faster.

### Stack

- Laravel back-end
- Vanilla JavaScript front-end
- Twitter's Bootstrap CSS framework

### Environment

- Linux environment
- Nginx web server
- MySQL database
- PHP back-end language

## Technical Requirements

This area shows all of the technical requirements corresponding to the various user requirements for this project. This will also detail out phases and which requirements will go into which phase.

- Play back video, and store a history, categorize the videos - Store the video in the YouTube channel (back up locally), will need a player that plays embedded YouTube videos, we want to work with the player to store run time information and we can store which videos that we have watched. Categories we can store with a pointer to the YouTube video link.
- Comments should linked to the YouTube video link as well as to the user who watched the video and / or made the comment.
- Likes or Dislikes will be 1 for likes, and -1 for dislikes. This is all we will store for this, except for the user who voted.
- Transcript is a future feature.
- User system:
  - Single Sign On is a future feature.
  - Database: The user system will use a database to store user information, such as email address, password, first name, last name, date joined, preferences for videos, technologies they have experience in, their career level, comment display name, country of residence, and technologies they want to learn.
  - Authentication: The user system will implement authentication to ensure that only authorized users can access the system. This will be done by checking the user's email address and password against the database.
  - Registration: The user system will allow new users to register for an account. This will involve providing their email address, password, first name, last name, and country of residence.
  - Profile Management: The user system will allow users to manage their profile information, such as their preferences for videos, technologies they have experience in, their career level, comment display name, and technologies they want to learn.
  - User Roles: The user system will implement user roles to control access to different features of the system. For example, users with the "admin" role may be able to manage other user accounts, while users with the "instructor" role may be able to create and manage video tutorials.
- User Favorites
  - Database: Store user favorites such as favorite tutorial videos, favorite series of videos. (Favorite sections of video transcripts to come later).
  - Favoriting: The user favorites system will allow users to favorite tutorial videos and series of videos. This will be done by providing a button or other mechanism that users can click to add an item to their favorites.
  - Viewing Favorites: The user favorites system will allow users to view their favorite items. This can be done by providing a dedicated page or section of the website where users can view all of their favorite items.
  - Removing Favorites: The user favorites system will allow users to remove items from their favorites. This can be done by providing a button or other mechanism that users can click to remove an item from their favorites.
- Additional System Requirements
  - Scalability: The user system and user favorites system should be scalable to support a large number of users.
  - Security: The user system and user favorites system should be secure to protect user data from unauthorized access.
  - Performance: The user system and user favorites system should be performant to provide a good user experience.
- Admin Panel will occur after initial release.
- Community Feedback
  - We need a contact form or a way to link to either specific videos or topics and to suggest improvements, or point out issues.
    - Store user information (email, user id).
    - Store topics (topic ids).
    - Store date and timestamp of when this form was submitted.
    - Store videos if any (video ids).
    - Store the user feedback.
    - Future feature (automatically create a ticket to resolve this / check if issue or improvement was already suggested).
  - We need a separate form to collect ideas or future features that we want to see in the application.
    - Store user information (email, user id).
    - Store date and timestamp of when this form was submitted.
    - Store the user feedback.
  - We need a third form for specialists or senior engineers to volunteer to take part in the learning center.
    - Store user information (email, user id).
    - Store date and timestamp of when this form was submitted.
    - Store an indication of what expertise user has (technologies they have experience in and career level).
    - Store user availability (we need the user to indicate when they would have time to volunteer).
    - Store user feedback (any languages that they want to do a video).
- Social connections
  - Provide the YouTube video link for copying so users can share videos with their networks.
  - Future functionality: LinkedIn / Facebook group pages

## User Requirements

- Video playback - We want to be able to watch the tutorial videos and match the resolution to our bandwidth capabilities. Watch, rewatch, or find other videos related to the most recently viewed video.
- Video storage - We need a way to store produced videos, we do not need to download them as they will be available online forever. We need them to be compressed and quickly decompress and view them, we may also want to encrypt / decrypt the videos to secure them for users of the site.
- Comments - Allow users to comment on other comments or the videos themselves.
- Likes or Dislikes - Allow users to like or dislike comments or videos themselves. If they like a video add that video to their favorites.
- Transcript - A full document transcript on the audio in the videos along with timestamps so that users can find specific parts of the video and rewatch or go back through the transcript to read through parts they want to review.
- User system - Single Sign On if possible, email as username, password, first name and last name, date joined, preferences for videos that they want to see over others, what technologies they have experience in, what level they are currently at in their career, also pick a comment display name, the country they reside in, and technologies they want to learn.
- User favorites - Favorite tutorial videos, favorite series of videos, or they can favorite a section in a transcript to highlight a particular segment of a video.
- Admin Panel:
  - Admin login - Admin login is locked down to moderators or admins only, create admin / moderator privilege for admins only.
  - Admin review new comments (AI assist to look for derogatory comments) - This is only for negative comments.
  - Admin upload new video - provide video title, series, series number (what part in the series is it), run time, and other related meta data.
  - Admin user management - Block users who keep making negative comments, add moderators, add additional admins.
  - Admin review community feedback - Add future features and issues / improvements to backlog, add volunteers to volunteer list.
- Community Feedback - Provide an area where users can suggest improvements to code, point out issues in existing code, suggest future features they want to see as a part of the Learning Center, or volunteer to take part in the Learning Center.
- LinkedIn / Facebook group pages, links for users to share with others to come to Learning Center site.

## Future Features

- Video Editing - this will allow us to edit sections of videos and splice them together to group them into a related topic, for example: if a video series goes in depth with Python and has a React front end, we may want to splice the Python parts together and the React parts together to form separate Python and React training modules.
- Education Module Creator - Provide a way for users to create training modules to help their fellow developers learn to code or learn to code at a higher level.
- Automated post creation for LinkedIn, Facebook, Pinterest, Instagram, Tiktok, and Twitter (if there are others feel free to mention them in the community feedback portal).
