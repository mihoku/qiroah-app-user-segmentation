# qiroah-app-user-segmentation
User Segmentation of Qiroah App using Duolingo Growth Model based on Markov Chain.

Using Duolingo Growth Model, users are categorized into the following user states based on their activity in the app: 

* Current Users measures the amount of users who are active in learning with Qiroah app today and also in the past week.
* New Users measures the amount of users who are experiencing Learning activities in Qiroah for the first time ever since installing the application.
* Reactivated Users measures the number of users who are active in learning with Qiroah app today, and the past month (30 days) but not in the past week (7 days).
* Resurrected Users measures the number of users who are active in learning with Qiroah app today, but the last time learning activity is more than 30 days ago (previously dormant).
* At Risk Weekly Active Users measure the number of users who are active in learning using Qiroah app in the past week (7 days) but not today.
* At Risk Monthly Active Users measure the number of users who are not active today, and the last learning activity was between 7 to 30 days ago.
* Dormant Users measure the number of users whose last learning activity was more than 30 days ago.
* Non-Learning Users measure the number of users who installed Qiroah app but never accessed and engaged with the learning content.

Since it is based on Markov chain, users transition between segments are also analyzed. For example as follows:

* Current User Retention Rate (CURR) which measures the daily rate of users in current learning users segment that stay in the same segment.
* New User Retention Rate (NURR) measures the daily rate of users in the New Learning Users segment that move up to the Current Users segment.
* Reactivated User Retention Rate (RURR) measures the daily rate of users in the Reactivated Learning Users segment that move up to the Current Users segment.
* Resurrected User Retention Rate (SURR) measures the daily rate of users in the Resurrected Learning Users segment that move up to the Current Users segment.
* Weekly Active User Retention Rate (WAURR) measures the daily rate of users in the At Risk Weekly Active Learning Users segment that move up to the Current Learning Users segment by starting a learning session.
* Reactivation Rate measures the daily rate of users in At Risk Monthly Learning Users segment that move up to Reactivated Users segment by starting a learning session.
* Resurrection Rate measures the daily rate of users in the Dormant Learning Users segment that move up to the Resurrected Users segment by starting a learning session.
* Weekly Users Loss Rate measures the daily rate of users in At Risk Weekly Learning Users segment that descend to At Risk Monthly Users segment.
* Monthly Users Loss Rate measures the daily rate of users in At Risk Monthly Learning Users segment that descend to Dormant Learning Users segment.
