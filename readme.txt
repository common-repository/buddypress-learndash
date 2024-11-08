=== BuddyPress for LearnDash ===
Contributors: buddyboss
Donate link: https://www.buddyboss.com/donate/
Tags: buddypress, learndash, lms, learning management system, learning, courses, courseware, education, social networking, activity, profiles, messaging, friends, groups, forums, notifications, settings, social, community, networks, networking
Requires at least: 3.8
Tested up to: 5.4.2
Stable tag: 1.3.0
License: GPLv3
License URI: http://www.gnu.org/licenses/gpl-3.0.html

BuddyPress for LearnDash integrates the LearnDash LMS plugin with BuddyPress, so you can add groups, activity, members, and forums to your courses.

== Description ==

Want your learners to interact with each other? **BuddyPress for LearnDash** turns your course driven website into a social education platform, creating a seamless bridge between BuddyPress and [LearnDash](http://www.learndash.com/).

= BuddyPress Groups =

Easily tie any LearnDash Course to a BuddyPress Group.

* Course participants automatically get added as members to the group
* Group becomes private to course participants and invited members
* Course Lessons become visible at the group
* Course activity gets streamed into the group feed (optional)
* Forum gets added to the group (if bbPress is enabled)
* Course featured image becomes group avatar (if no group avatar has been set)

= BuddyPress Activity =

Activity is one of the core features of BuddyPress, allowing users to interact with each other in real-time. When a course is tied to a group, course actions are optionally added to the group’s activity stream. Group admins can determine which actions to allow in their group, including:

* User starts a course
* User completes a course
* User creates a lesson
* User completes a lesson
* User passes a quiz
* User comments on single lesson page

= BuddyPress Members =

* Your members can view their Active and Completed courses in their profiles.
* Leaders and Students get added as filterable tabs in your Members directory.
* All LearnDash user links redirect to member profiles (instead of author pages).

= bbPress Forums =

If bbPress is enabled, a forum will be tied to every “course group” automatically, using the same name as the course for the forum title. Group members can then discuss the course in one central location.

= Extend LearnDash with 'Social Learner' =

BuddyPress for LearnDash is built by the experienced developers at BuddyBoss who also offer a premium social learning solution called [Social Learner](https://www.buddyboss.com/product/social-learner-learndash "Social Learner for LearnDash").

== Installation ==

= Before Installing =

1. Make sure you have [LearnDash](http://www.learndash.com/) installed and activated.
2. Make sure you have [BuddyPress](https://wordpress.org/plugins/buddypress/) installed and activated.

= From your WordPress dashboard =

1. Visit 'Plugins > Add New'
2. Search for 'BuddyPress for LearnDash'
3. Activate BuddyPress for LearnDash from your Plugins page.

= From WordPress.org =

1. Download BuddyPress for LearnDash.
2. Upload the 'buddypress-learndash' directory to your '/wp-content/plugins/' directory, using your favorite method (ftp, sftp, etc...)
3. Activate BuddyPress for LearnDash from your Plugins page.

= Configuration =

1. Enable 'User Groups' at 'Settings > BuddyPress > Components'
2. Enable Forums for Groups by downloading [bbPress](https://wordpress.org/plugins/bbpress/).
3. Visit 'Settings > BP for LearnDash' and select your desired options.

== Frequently Asked Questions ==

= Does it come with the LearnDash plugin? =

No, it does not. You will need to purchase [LearnDash](http://www.learndash.com/) separately.

= Where can I find documentation and tutorials? =

For help setting up and configuring any BuddyBoss plugin please refer to our [tutorials](https://www.buddyboss.com/tutorials/).


= Does this plugin require BuddyPress? =

Yes, it requires [BuddyPress](https://wordpress.org/plugins/buddypress/) to work.

= Will it work with my theme? =

Yes, BuddyPress for LearnDash should work with any theme, and will adopt your BuddyPress styling along with CSS from the LearnDash plugin. It may require some styling to make it match perfectly, depending on your theme.

= Does it come with a language translation file? =

Yes. Want to translate BuddyPress for LearnDash into your own language? We'll be happy to add your translation into the plugin :)

= Where can I request customizations? =

For BuddyPress customizations, submit your request at [BuddyBoss](https://www.buddyboss.com/buddypress-developers/).

== Screenshots ==

1. **Course Group** - Associate LearnDash courses with BuddyPress groups.
2. **Course Group Settings** - Add a course to a BuddyPress group and configure its activity actions.

== Changelog ==

= 1.3.0 =
* Fix - Fix fatal error when group component is not activated
* Fix - Some code improvements
* Tweak - Added check for Activity component

= 1.2.9 =
* Fix - Group and Course connectivity data is getting removed when uninstaiing plugin
* Tweak - Added Russian translation files
* Tweak - Added filter for LearnDash group discussion button

= 1.2.8 =
* Fix - Users Enroll message when updating course from Classic & Gutenberg editor
* Fix - Child theme template path

= 1.2.7 =
* Fix - Fatal when BuddyPress Group component disabled
* Fix - Removed LearnDash deprecated function

= 1.2.6 =
* Fix - Fatal when BuddyPress Group component disabled.
* New - Tested with WordPress 5.2.1


= 1.2.5 =
* Fix - Gutenberg editor compatibility
* Fix - Cannot set a group public when it is linked with the Course
* Fix - Leave off group enrollment if course has no buddypress group attached
* Fix - If group is public then Course Activity are not appearing on Site- wide Activity page
* Fix - Forbid translation of the buddypress profile courses menu slugs
* Fix - Global Search out of memory issue fix
* Fix - FATAL error occurs while saving/updating the course if course has group attached
* Fix - FATAL error on single group page after BuddyPress 3.0 update
* Fix - PHP Warnings

= 1.2.4 =
* New - Clean up on the plugin uninstall. Deletes options, course activities, group, and course link
* Fix - Detach group from the course when group is deleted
* Fix - PHP Fatal error on activity page if group component is disable
* Fix - Make Learndash activities action translatable
* Fix - Make Learndash activities action translatable
* Fix - Fixed Fatal error on removing course from Learndash group

= 1.2.3 =
* Fix - Edit Course page throws error if "Course Access List" field is empty in the meta box.

= 1.2.2 =
* Tweak - Student access list update logic tweak
* Fix - Single activity page is blank for some group activities
* Fix - Course settings inside group should not be accessible for the student
* Fix - removed group activation check
* Fix - Unclosed div tag in templates/courses.php
* Enhancement - bp_learndash_user_courses filter added
* Enhancement - Add or remove member from the buddypress group on a course access update
* Fix - LD group enrolment fix
* Fix - group activity user_id fix
* Fix - User removal from group when removed from course
* Enhancement - bp_learndash_user_courses_atts filter added
* Fix - Fatal error whilst adding new course


= 1.2.1 =
* Fix - LearnDash v2.3 compatibility
* Fix - Multisite fixes
* Fix - Whole network crashes when activating BP LearnDash on main site
* Fix - Students are not getting added into the course buddypress group while doing course mass enrolment
* Fix - Members removal from a related BuddyPress Course Group happens after a course is updated or changed
* Fix - Hidden groups are not displaying in group meta box on course edit page
* Fix - Statistic column added under Profile > My Courses

= 1.2.0 =
* Fix - Hidden groups are not displaying in group meta box on course edit page
* Fix - Students are not added into the course-group while doing course mass enrolment
* Fix - Can not upgrade user's group role to Administrator
* Fix - Member removal from a related course-group happens after a course is updated or changed
* Fix - Multisite’s issues
* Fix - PHP7 compatibility
* Fix - PHP errors

= 1.1.0 =
* Fix - Infinite loop on saving course with attached course
* Fix - Problem with WordPress 4.4.2/4.5 - admin panel
* Fix - Gateway timeout problem

= 1.0.7 =
* Fix - Group/forum registration not working while manually adding student to course
* Fix - Moved button under quizzes, instead of under lessons
* Fix - LearnDash custom labels compatibility
* Fix - Check if BuddyPress is installed and activated
* Fix - Check if LearnDash is installed and activated
* Fix - Course group experiences
* Fix - PHP warning

= 1.0.6 =
* Fix - Duplicate forum getting created when updating course
* Fix - Group/forum registration not working with group enrollment
* Fix - BP Reorder Tabs compatibility

= 1.0.5 =
* Fix - Create forum only if checked
* Fix - Add group activity if comment posted on topics
* Fix - Hide lessons and topics from users if they don't have access to the parent course
* Fix - Correctly turn off course group activities according to settings
* Fix - When on Course Group Forum, the Course page should go back to the course, but not the group
* Fix - Changed no course found message string
* Fix - Made the courses tab in a group always point to single course page

= 1.0.4 =
* Added missing translation strings

= 1.0.3 =
* Fixed content missing in single course if no group is attached
* Removed course discussion button for non-students

= 1.0.2 =
* Topics and Lessons now link back to Course group
* Added filter for Course page title
* Added Course expand/collapse links

= 1.0.1 =
* Updated readme

= 1.0.0 =
* Initial public release
